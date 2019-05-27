This is a git repo built solely for testing purpose.
*Please ignore it.*

## How To Play : 

 #### 1. Setup :
* Download Game.c file 
* Compile on linux machine using gcc compiler by running the command
```  gcc Game.c  ```
  * In case you get error like ```gcc not found, but can be installed with ...``` run the following command
  ```sudo apt install gcc```  followed by entering your password. This command installs gcc compiler on your machine, which is important for compilation of Game.c file.
* After installing and compiling, make sure an object file named a.out is created in your current directory. This can be done either manually or using the command ``` ls | grep a.out ```. This basically lists out every file and folder in your current working directory and searches for a.out named file .
   * Note that you can choose any other name for your object file using ``` gcc -o FILE_NAME Game.c``` where FILE_NAME is the custom name that you want to give to your object. The default file name is given a.out.
* Now once the object file is created, simply execute your object file using ```./a.out```. This commands excecutes an executable file named a.out in current directory.
* The details of playing are provided below. In case you like the game but don't like to go the specific directory every time to compile and execute, you may add the compiled object file to the path of environment variables. Follow the below steps for the same : 
    
    #### Make the game accessible from any directory :
    *
