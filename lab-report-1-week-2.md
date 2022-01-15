# Hello new CSE 15L Students!!

In this tutorial, I'm going to be walking through the steps of installing the IDE VIsual Studio Code to your computer/laptop. I'm currently on a Mac so most of this tutorial is going to be adjusted for people on Mac. I'm also going to be explaining how to log into servers in the basement of the CSE building at UCSD. Specifically, I'm going to be logging into the account ieng6 and remotely connecting to it.

<p>&nbsp;</p>

## 1) Installing Visual Studio Code

- The first thing we want to do is to install the IDE, Visual Studio Code onto our computer. You can go to this link here [Install VS Code](https://code.visualstudio.com/Download)
- After successfully installing Visual Studio Code, you can open it and your screen should like the second image.

![lab-report-1-week-2.md](https://user-images.githubusercontent.com/86133628/149597476-52ee2a89-f7a1-4457-a870-14c015c08013.png)

![lab-report-1-week-2.md](https://user-images.githubusercontent.com/86133628/149601443-e36f56e6-92b5-46be-be16-f02fb34376aa.png)





<p>&nbsp;</p>

## 2) Remotely Connecting

- We want to remotely connect to the server in the basement of the UCSD CSE building and in order to do that we will use the `ssh` which stands for secure shell copy
- We first want to open a terminal. We could do this by going to Terminal > New Terminal.
- In the terminal, we want to type the command `ssh cs15lwi22agy@ieng6.ucsd.edu`. The letters agy will be repalced with your own username which can be found here [Finding username](https://sdacs.ucsd.edu/~icc/index.php). After logging in, your screen should look like the image below.

![lab-report-1-week-2.md](https://user-images.githubusercontent.com/86133628/149598456-fdb37d9d-a45e-42e6-9c7b-2bf2a4b696a3.png)


## 3) Trying Some Commands
- Once we're in, we could use commands like `ls` to list the files in the directory.
- We could also use a command like `cd` to change directories.<img width="926" alt="image" src="https://user-images.githubusercontent.com/86133628/149601996-9050da35-5487-4e4e-b4bb-e4ca9ef8e562.png">

- Here is an image of some commands I tried while in ieng6.

![lab-report-1-week-2.md](https://user-images.githubusercontent.com/86133628/149598948-56c0531a-4eea-4492-b30a-38f9a6efa9e8.png)



## 4) Moving Files with Secure Copy `scp`

- Next, we want to find a way to move our files on our computer the client, to the server and we could do this by running the command `scp WhereAmI.java cs15lwi22zz@ieng6.ucsd.edu:~/`, where the file WhereAmI.java could be any file name.
- Here, I create a file named WhereAmI.java and secure copy it to ieng6.
- Your terminal should show 100% when the file has been successfully copied.

![lab-report-1-week-2.md](https://user-images.githubusercontent.com/86133628/149600534-c50090e4-7291-4b6c-8c50-8bec4fba0c3f.png)

![lab-report-1-week-2.md](https://user-images.githubusercontent.com/86133628/149600533-b5a8ae1a-cee1-4066-9205-8ee2a66c6462.png)

## 5) Setting an SSH Key

- It could be time consuming every time we want to sign in we have to input our password.
- We could use an SSH key to skip the password and sign in automatically
- This saves us a lot of time and your screen should look like the image below.

![lab-report-1-week-2.md](https://user-images.githubusercontent.com/86133628/149600867-9d0c6f0e-35ed-401f-aa0c-2cfe90e981e9.png)


## 6) Optimizing Remote Running

- In order to make our lives easier and faster, we can run multiple commands at once.
- Instead of always signing in first then using a command like `ls`. We could do these steps simultaneously
- We could do this by runnning the command `ssh cs15lwi22@ieng6.ucsd.edu "ls"` where "22" is replaced with your unique username. This command will sign you in and list the files.

![lab-report-1-week-2.md](https://user-images.githubusercontent.com/86133628/149601247-89f92998-878d-41a3-b227-db2b79996910.png)



