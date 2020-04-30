# ***Creating instance on AWS Cloud*** #

* Instances are nothing but a virtual machine with computing resources, available over the cloud.
* We can use this instace for creating a virtual server machine which can be made using virtually available resources and can be accessed remotely. This machine can act exactly like the physical server without the need of physica hardware, this means, we can use aws instance as web server for host websites or a ftp server  for file storage security and management or a mail server for management and configuration of corporate E-mail accounts and all the other types of servers.
* To create an instance:
  * Go to Services.
  * Under the 'compute' section, click on the instance type you want(EC2 in our case).
  * If you already have an instance running, click on running instances otherwise skip this step
  * Click on 'Launch Instances', under 'Launch Instances' section. 
  * Select the image type(OS) you want to be installed on the instance.
  * On the next page, select the type of intance, that is, the amount of resources(CPU,DIMMs,etc.) you want for your instance.
  * Enter the configuration details and move forward to add storage on the instance.
  * Select the amount and type of storage you want.
  * Next step is to add any tags if you want.
  * Final is to configure the firewall. We can use the default firewall setting or alter them if we want.
  * Now we have to review all the settings and finally launch the instance using an existing Key or we can create a new key.