# CSE 15L Lab Report #2


In the lab this week we worked on systematic testing, we also worked on committing changes to our code in the file `MarkdownParse.java`. Our team fixed bugs
in our code in order to allow for more inputs in our test files. On this page I'm going to be showing some of the changes that we made to our code as well
descriping the input of our failing induced input. In the end, for each bug that we fixed, I will be giving a brief explanation of the relationship between the
the bug, the symptom, and the failure-inducing input.


## 1) Bug Fix#1

![Bug Fix 1](https://user-images.githubusercontent.com/86133628/151572597-47863110-21f2-4a79-ad9c-fd6abc470c73.png)
<p>&nbsp;</p>

Here I'm attaching a link to a txt file where I have the failure inducing input,[Bug #1 Input](https://github.com/cpareja3025/cse15l-lab-reports/files/7962529/testfile2text.txt), I'm also attaching a screenshot of my terminal when I'm running the program with
this input. This is called the symptom of the failure-inducing input.
<p>&nbsp;</p>

![Symptom#1](https://user-images.githubusercontent.com/86133628/151638038-6d217bb8-0a35-4cc7-8a07-1ec60138c060.png)

In this failure-induced input we noticed that the original `MarkdownParse.java` program had a bug if we added text after the link in the markdown file. This why we added the if statement with  `nextOpenBracket == -1` then we break. This symptom allowed us to realize that the program is looking for a bracket and when we gave it text after the link, the program failed.



## 2) Bug Fix#2
![Bug Fix 2](https://user-images.githubusercontent.com/86133628/151573069-9e1175a6-34b6-462b-891d-b11fa476c6c7.png)
<p>&nbsp;</p>

Here is the link to the failure-inducing input and below is the symptom of the bug. I'm also attaching an image of the symptom of my terminal when I run the
program with the failure-induced input.[Bug #2 Input](https://github.com/cpareja3025/cse15l-lab-reports/files/7962587/break2txt.txt)
<p>&nbsp;</p>

![Symptom#2](https://user-images.githubusercontent.com/86133628/151638533-1e975cc5-2402-48f7-85e2-ce8423cf87f9.png)

In this failure-induced input we noticed that the original `MarkdownParse.java` program had a bug if the link had parantheses. The program didn't crash
but we were getting a logic error. We noticed that the entire link wasn't being printed. Therefore, we fixed this bug by adding an `if` statement if a link with parantheses is inputted. 



## 3) Bug Fix#3
![Bug Fix 3](https://user-images.githubusercontent.com/86133628/151573232-ad25f2ee-828f-41de-9c5a-b52b516461c2.png)
<p>&nbsp;</p>

Here is the link to the failure-inducing input and below is the symptom of the bug. [Bug#3 Input](https://github.com/cpareja3025/cse15l-lab-reports/files/7962597/break3txt.txt). I'm also attaching an image of the symptom of my terminal when I run the program with the failure-induced input.
<p>&nbsp;</p>

![Symptom#2](https://user-images.githubusercontent.com/86133628/151639068-475f3e28-1288-4f7a-a143-e15d6f6364ee.png)


In this failure-induced input we noticed that the original `MarkdownParse.java` program had a bug if we inputted an image instead of link. The program did not crash but the symptom was obvious for us as the program was only outputting `[]` and not the link which was accidently inputted in markdown as ![] for images instead of `[]` for links. 


