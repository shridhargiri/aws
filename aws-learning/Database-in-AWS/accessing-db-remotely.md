## ***Acessing the **MYSQL** database remotely*** #
- Any remote client can be used to access the remotely located MySQl server or database.
- There are broadly two types of MySQL clients available:
    1. IDE(Integrated Development Environment) based client.
    2. GUI(Graphical User interface) based client.

- The IDE and GUI based client for windows can be directly downloaded from [MySQL's official website](https://dev.mysql.com/downloads/installer/).
- When on Linux Operating systems, IDE clients are more commonly used.
- To install MySQL on a Linux system, follow the steps:
    1. Frist of all, MySQL package need to be installed. To do so, type the command:
        `sudo apt-get install mysql-server`
    2. Once this package is installed, we need to run MySQL Utilities, where we can set the root password for our local database in mysql  and configure other elements of our package. MySQl utilities can be accessed using the following command:
        `sudo mysql_secure_installation utility`
    3. After the configuration set-up is completed, we can allow MySQL through our system's Firewall, doing which we would be able to access our local databases using a remote machine.
        `sudo ufw enable`
        `sudo ufw allow mysql`
        These are the commands to allow MySQL through the firewall.
    4. Finally, we need to start the MySQL service on the system using 
        `sudo systemctl start mysql`
    5. If we want the service automatically start on evevry boot:
        `sudo systemctl enable mysql`
    6. That's it, now MySQL service is running on the system and to access any database use the following command:
        `mysql -u <username> -h <server ip address>`

        Example: mysql -u root -h 0.0.0.0

    7. If the local database needs to be accessed, enter `localhost` in the section where server ip address needs to be entered.