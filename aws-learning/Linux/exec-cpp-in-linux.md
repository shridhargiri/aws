### ***How to execute C++ programs in Linux Operating System*** #
* Here, we'll be using the GCC compiler for executing the programs in Linux.
* There is a package available in Linux repositories which goes by the name 'G++'. This package(Software in linux) is used to compile C/C++ programs and create an object file. Once this object file is created, the linux system is able to run this file directly.
* This package needs to be installed on the system to proceed and it can be done using the following command:
        `sudo apt-get install g++`
* Here, `apt-get` is the command used to install, update or remove packages in Linux systems. [Here](https://www.computerhope.com/unix/apt-get.htm) you can read more details for this command.
* We use `sudo` because to run `apt-get`, we need root privilege and root privilages can be attained when user is a Super User in linux. Hence the name sudo(Super User do).
* In the last, `install` is the operation performed by the command `apt-get` on the package `g++`.

    **Note:** If there is an error that the package doest not exist after executing the above command, run the following command first:
        `sudo apt-get update`
    This updates the list of packages available in the local repository of Linux Operating System.
    Once this is done successfully, re-run the install command.
* Now, to compile a c++ program follow the below syntax:
        `g++ <filepath/filename.cpp>`
* This would execute the cpp file with the specified file name at the specified location and an object file with the name `a.out` would be created.
* Now, execute the object file to run your program. To execute, when on directory containing the object file, enter the following command:
        `./a.out`
* Object file is by default created in the current working directory.
* If the path and name of the on=bject file needs to be specified, follow the following syntax:
        `g++ -o <objectfilepath/objectfilename.out> <filepath/filename.cpp>`
* Now, run the object you created.
