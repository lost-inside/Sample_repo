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
* The details of playing are provided [below](####-2.-play-). In case you like the game but don't like to go the specific directory every time to compile and execute, you may add the compiled object file to the path of environment variables. Follow the below steps for the same : 
    
    #### 1.1 Make the game accessible from any directory :
    * Compile Game.c file using the steps explained above using a name other than a.out . The other name is important so that in future if you compile and run some other code, your machine is not confused as which a.out should be executed. 
    * Run the following command ```sudo mv FILE_NAME /usr/bin/``` and then enter your password if required. This basically moves your object file to a directory named bin where many globally accessible executable files are stored. 
    * Now you can execute your object file from any location by just typing FILE_NAME on your command line.
    * Anytime you feel to remove the file from the folder of globally executables, type the following command 
    ``` sudo rm /usr/bin/FILE_NAME ``` followed by your password. Note that after using this command, you will no longer be able to run your object file from any director just by typing FILE_NAME on the command line unless you add the file to any one of the locations contained in PATH variable. More details about PATH variable can be found [ here ]( https://stackoverflow.com/questions/37676849/where-is-path-variable-set-in-ubuntu ).
    
    
    
 #### 2. Play :
   * The game requires two players who have to enter their name after executing the object file. The first three letters of their name should be diffrent to avoid confusion.
     ##### 2.1 Rules :
        * The first player to enter name takes first turn and then both play alternate turns. 
        * In this version of game, there are 5 rows and 5 columns. The player has to pick a column that isn't full. The lowest empty space in that column will be occupied by him.
        * The first player to occupy any 4 consecutive places in any 8 possible direction wins. 
        * In case of tie, no player is declared winner.
        * ![Screenshot from 2019-05-07 17-15-58](https://user-images.githubusercontent.com/49042740/58409514-d8f21a80-808d-11e9-9cdd-becaa104a212.png)
