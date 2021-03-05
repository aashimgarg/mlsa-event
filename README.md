# ➡Getting started with Git 🎉 and Github🐙


### Topics
- [What is Git?](#1)
- [What is Github?](#2)
- [Installation?](#3)
- [Setting up git in your device](#4)
- [Setting up a local repo](#5)
- [Creating a remote repo](#6)
- [git-remote](#7)
- [Staging changes to remote](#8)
- [git-branches](#9)
- [git-rebase](#10)
- [How to contribute to open-source projects](#11)
- [Working with Github Actions](#12)
- [Cheat-Sheet](#13)

### Got a query?
Feel free to reach us in case of any queries. We are always happy to help you one bit at a time🐱‍💻

###### Aashim Garg


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

### Installation

With platform specific installers for Git, GitHub also provides the ease of staying up-to-date with the latest releases of the command line tool while providing a graphical user interface for day-to-day interaction, review, and repository synchronization.

1. GitHub for Windows
https://windows.github.com

2. GitHub for Mac
https://mac.github.com

For Linux and Solaris platforms, the latest release is available on the official Git web site.

3. Git for All Platforms
http://git-scm.com

### Setup

Configuring user information used across all local repositories

```
git config --global user.name “[firstname lastname]”
[set a name that is identifiable for credit when review version history]

git config --global user.email “[valid-email]”
[set an email address that will be associated with each history marker]

git config --global color.ui auto
[set automatic command line coloring for Git for easy reviewing]
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

#### Tracking Path Changes

Versioning file removes and path changes

```
git rm [file]
[delete the file from project and stage the removal for commit]
```
```
git mv [existing-path] [new-path]
[change an existing file path and stage the move]
```
```
git log --stat -M
[show all commit logs with indication of any paths that moved]
```

#### Share and Update

Retrieving updates from another repository and updating local repos

```
git remote add [alias] [url]
add a git URL as an alias

git fetch [alias]
fetch down all the branches from that Git remote

git merge [alias]/[branch]
merge a remote branch into your current branch to bring it up to date

git push [alias] [branch]
Transmit local branch commits to the remote repository branch

git pull
fetch and merge any commits from the tracking remote branch
```

#### git-rebase

<img src="https://wac-cdn.atlassian.com/dam/jcr:01b0b04e-64f3-4659-af21-c4d86bc7cb0b/01.svg?cdnVersion=dt" />

It solves the same problem as git merge. Both of these are used to add changes from one branch to another. The only difference is 


```
git checkout -b feature-branch

[add commits to your feature branch]

git rebase master
```

### Contributing to open-source
![Untitled Diagram](https://user-images.githubusercontent.com/44068102/107565039-2e2ae280-6c09-11eb-98e5-d738d4a06d33.png)


### Github Actions <sup style="font-size: 15px">[Source](https://docs.github.com/en/actions/learn-github-actions/introduction-to-github-actions)</sup>

![ga](https://repository-images.githubusercontent.com/200244092/c64f8080-586d-11ea-9f2b-fc72525069dd)

GitHub Actions make it easy to automate all your software workflows. Github Actions let you build, test, and deploy your code right from GitHub. You can also assign code reviews, manage branches, and triage issues the way you want with actions.

Every Github action required a <code>.yml</code> file.

#### Components 
- Workflow: The workflow is an automated procedure that you add to your repository. Workflows are made up of one or more jobs and can be scheduled or triggered by an event.

- Events: An event is a specific activity that triggers a workflow.

- Jobs: A job is a set of steps that execute on the same runner. By default, a workflow with multiple jobs will run those jobs in parallel. 

- Steps: A step is an individual task that can run commands in a job. A step can be either an action or a shell command. 

 ➡ [Demo Project](https://github.com/saranonearth/demo)


[Get Started Here](https://lab.github.com/githubtraining/github-actions:-hello-world)🔥

### Cheat Sheet

- How to edit a git commit?
```
git commit --amend
```
- Better ways to see git log?

```
git log --oneline
git log --graph
```
- I want to check a PR locally before mergin
```
git fetch origin pull/$ID/head:$BRANCHNAME && git checkout $BRANCHNAME
```
- I want to select specific commits from a PR
```
git cherry-pick commit-hash
```
- How do I add a remote?
```
git remote add [name | example: origin,upstream] "url of repo"
```
- How do I view all my remotes?
```
git remote -v
```
- Can I remove a remote?
```
git remote rm origin,upstream etc
```
- How do I pull from remote?

```
git pull origin branch-name
```
- I staged my changes by mistake. What can I do now?

```
git reset
```

- I am trying to pull but getting "fatal: Not possible to fast-forward, aborting." error

```
git pull -f origin 'branch-name'
```
