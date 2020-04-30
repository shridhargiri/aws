## Accessing the AWS instance remotely #
   - The instance that we have made earlier can be accessed using any remote computer.
   - Windows instance can be accessed using remote desktop client on the computer which is used for accessing the instance.
   - But here for the linux instance, we are using a software, MobaXterm to access the linux instance.
   - Here are the steps:
     1. Open MobaXterm software
     2. Click on session(Top left corner)
     3. Here select the port using which the connection is to be made(SSH in our case).
     4. Enter the public IP of instance in the 'Remote Host section'.
     5. Username can also be specified in advanced so it would not be asked later.
     6. Under advanced SSH settings, add the private key used for the instance.
     7. Click on 'Okay'.

   - Now, if the connection is successful, terminal of linux would be launched in the software's console.
   - This is the linux instance's terminal that we have created.

##### In this way an AWS instance can be accessed #