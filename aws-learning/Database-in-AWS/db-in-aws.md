## ***Databases in AWS*** #
- AWS provides many different types of database services. Relational databases are also provided by AWS under the name, RDS(Realional Database services).
- Under the RDS service, AWS provides the following database engines to choose from:
  - [Amazon Aurora](https://en.wikipedia.org/wiki/Amazon_Aurora)
  - MySQL
  - MariaDB
  - PostgreSQL
  - Oracle
  - Microsoft SQL server

Using AWS RDS service provides all the common AWS benefits and along with those benefits, the responsiblity of tasks such as autobackup, security and maintenance is also undertaken by AWS.

### *Creating a MySQL database in AWS* #
- As this is a service provided by AWS, we need to head towards the 'Services' menu in our AWS console.
- Under the 'databases' section, type of the database that need to be created can be selected.(RDS in our case)
- Once on the Amazon RDS Dashboard, click on 'Create Database'.
- Here, there are two methods to create a database, one is 'Standard create' and the second is 'Easy create'. In 'easy create' mode, AWS automatically selects most commonly used and most recommended configuration and creates the database.
- Select 'Standard create' as we'll manually configure all the configuratioons in the database.
- Next option is to select the Engine type. Above mentioned engine type are available for use, here, select MySQL.
- Just below the engine types, the version of Engine type can also be changed. Choosing the version depends upon the purpose of using this database because different database engine version have different compatiblity issues.
- Next step is to select the sample template for any specific use case. In our case, we'll select 'Free tier' because we are doing this for a hands-on experience with AWS databases.
- Next is the section where we can configure the properties of our database such as Database name, username and password. Set them accordingly
- Database instance size:
  - Database is nothing but a physical server running the database software. 
  - In case of AWS, a virtual instance hosts the database software and it can be accessed remotely.
  - Therefore we need to select the instance type and size, that is, RAM and CPU for our database.
- Once the instance type is selected, next is the most important part in a database, the seze of DB.
- We need to seelct the storage type and storage size we want to allocate to our Database. AWS also takes care of the situation where our database may run out of storage. In such situation, our database can expand upto the maximum thershold limit automatically.
- Apart from this AWS also provides and additional feature here known as Storage auto-scaling. If this feature is turned on, the storage limit of our database would be automatically expanded even if we have even reached the specified threshold limit.
- In the connectivity section, you can change or create a new VPC if you want a different subnet configuration for your database.
- Along with this if you want to access the database outside the AWS VPC, select additional connectivity configuration.
- Under the 'Publicly accessible' option, select 'Yes'.
- That's it all the other options can be kept default accordingly or we can also review all the addtional options and make changes.
- It takes a couple of minutes for the new database to be created and initialized.