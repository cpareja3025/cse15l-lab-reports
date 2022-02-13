# Lab Report 3 Week #6
 > In this weeks Lab Report, I will be explaing the steps to remotely copying the `markdownparse` repository to the ieng6 server at the UCSD CSE basement. I will be walking through the steps of choice #3 from the week 5 lab. In order to do this we need to run certain commands such as `scp -r` to successfully copy the repository.


## 1) Copying Markdown Parse to your personal ieng6 account

![scp repo to remote server](https://user-images.githubusercontent.com/86133628/153771294-976c5d82-8850-4988-bcaa-865caad4ed5b.png)
<p>&nbsp;</p>
In order to copy the markdownparse repository on your computer to a remote server such as ineg6 at UCSD, we first need to run the commmand `$ scp -r . cs15lwi22abc@ieng6.ucsd.edu:~/markdown-parse` where `abc` is your personal username to log into the ieng6 server which you could look up here 
[Account Lookup](https://sdacs.ucsd.edu/~icc/index.php) . In the image above we see each file and directory in the repository being successfully uploaded to your ieng6 account.

<p>&nbsp;</p>



## 2) Running JUnit Tests on ineg6

![Running JUnit Tests](https://user-images.githubusercontent.com/86133628/153771339-c6f43e7b-0a49-4a5f-9408-99d5a19081f0.png)
<p>&nbsp;</p>
In order to run the Junit Tests on ieng6 we first need to make sure that we have all of the neccessary files to run the Tests. We need to make sure we have the `MarkdownParse.java`, `MarkdownParseTest.java` as well as the directory `lib` where we have all of the JUnit files in order to be able to run the tests. After checking we have all of these files and directories using the `ls` command in the termninal, we can now run the commands to run our JUnit Tests on ieng6. In the image above we see that all of the tests ran successfully and there was no errors on ieng6 with these JUnit tests.

<p>&nbsp;</p>
