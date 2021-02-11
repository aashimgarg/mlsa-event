# ➡Getting started with Git 🎉 and Github🐙


### Topics
- [What is Git?](#1)
- [What is Github?](#2)
- [Setting up git in your device](#3)
- [Setting up a local repo](#4)
- [Creating a remote repo](#5)
- [git-remote](#6)
- [Staging changes to remote](#7)
- [git-branches](#8)
- [How to contribute to open-source projects](#9)
- [git-rebase](#11)
- [Working with Github Actions](#12)

### Got a query?
Feel free to reach us in case of any queries. We are always happy to help you one bit at a time🐱‍💻

###### Aashim Garg
<div style="display:flex">
<div style="width:20%">
<img src="https://www.google.com/imgres?imgurl=https%3A%2F%2Fmedia-exp1.licdn.com%2Fdms%2Fimage%2FC4E03AQED3YUDxZR_SA%2Fprofile-displayphoto-shrink_200_200%2F0%2F1610032551253%3Fe%3D1616025600%26v%3Dbeta%26t%3DoZvDVpRiDV3s7sGWC1cHze51Z4oJTTJneXlFvsgYK4o&imgrefurl=https%3A%2F%2Fin.linkedin.com%2Fin%2Faashim-garg-370104198&tbnid=GDULG23uTLwzfM&vet=12ahUKEwjQ8qPY4NruAhXMDLcAHfhSAwAQMygBegQIARAo..i&docid=D6hlV03FTJJqqM&w=200&h=200&q=aashim%20garg&client=ubuntu&ved=2ahUKEwjQ8qPY4NruAhXMDLcAHfhSAwAQMygBegQIARAo" style="border-radius:100%" /> </div>
<div>

<a href="https://www.linkedin.com/in/aashim-garg-370104198/">&nbsp;&nbsp;🔗LinkedIn</a>
<a href="mailto:aashim1garg@gmail.com">&nbsp;&nbsp;📧Email</a>

###### Saran
<div style="display:flex">
<div style="width:20%">
<img src="https://media-exp1.licdn.com/dms/image/C5603AQFVab5Kbi2x7w/profile-displayphoto-shrink_100_100/0/1612096633101?e=1618444800&v=beta&t=brEmn-KGIXc2W8sOAlBNZ-mX7eLD9yExV9xes2XONqA" style="border-radius:100%" /> </div>
<div>

<a href="https://www.linkedin.com/in/saranonearth/">&nbsp;&nbsp;🔗LinkedIn</a>
<a href="mailto:saran.suresh@outlook.com">&nbsp;&nbsp;📧Email</a>

</div>
</div>

#### What is Git

Git is the free and open source distributed version control system that's responsible for everything GitHub related that happens locally on your computer.

#### What is GitHub

GitHub is a code hosting platform for collaboration and version control. GitHub lets you (and others) work together on projects.


#### git-rebase

<img src="https://wac-cdn.atlassian.com/dam/jcr:01b0b04e-64f3-4659-af21-c4d86bc7cb0b/01.svg?cdnVersion=dt" />

It solves the same problem as git merge. Both of these are used to add changes from one branch to another. The only difference is 


```
git checkout -b feature-branch

[add commits to your feature branch]

git rebase master

```

#### Setting up a local repo

1. Open Terminal.
2. Change the current working directory to your local project.
3. Initialize the local directory as a Git repository.

```
git init -b main

```

4. Add the files in your new local repository. This stages them for the first commit.
```
git add .

```
5. Commit the files that you've staged in your local repository.

```
git commit -m "First commit"

```
6. At the top of your GitHub repository's Quick Setup page, click to copy the remote repository URL.

7. In Terminal, add the URL for the remote repository where your local repository will be pushed.

```
git remote add origin  <REMOTE_URL> 

```
8. Push the changes in your local repository to GitHub.
```
git push origin main

```


