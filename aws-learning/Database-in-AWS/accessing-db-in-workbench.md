## ***Accessing AWS RDS in Workbench application*** #
- The MySQL RDS created in AWS can be accessed using workbench application.
- Workbench is a GUI(Graphical User Interface) based application used to access and manage MySQL databases available on the local machine or on a remote server.
- Here, we will use workbench application to connect and manage the MySQL RDS available on the AWS cloud.
- Following are the steps to get the workbench application connected to the remote SQL:
    1. Download the workbench application from [MySQL Official website](https://dev.mysql.com/downloads/workbench/) and install it.
    2. Now login to the AWS account and navigate to the RDS section.
    3. Once on the RDS section in AWS console, click on "DB Instances" and select the database that you want to use.
    4. Here, make a note of endpoint URL and the port number under the 'Connectivity & security' tab.
    5. Open workbench application and click on the `+` icon infront of `MySQL Connections` to add connection with the remote server.
    6. Under the '**Connection Name:**', enter any name of your choice.
    7. Enter the endpoint URL available from the RDS section on AWS console in the '**Hostname:**' textbox.
    8. Final step is to enter the login details of the MySQL database.
    9. To do so, enter the username and for the password, it needs to be saved into the vault.
    10. Therefore, click on '**Store in vault ...**' button infront of '**Password:**' and enter the database password in the blank textbox available.
    11. Once all these steps are completed, we can check if the details entered by us are correct or not by clicking on '**Test connection**' button.
    12. Now click on '**OK**' to save this new connection.
    13. Now, to access the remote database, simply double click on the connection name available under '**MySQL Connections**' in workbench.