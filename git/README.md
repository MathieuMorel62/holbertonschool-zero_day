# <p align="center">GIT</p>
<img src="https://www.biteinteractive.com/wp-content/uploads/2021/05/git-vs-github.png" width="100%">

## Description
### Git & Github

Git and GitHub are essential tools for managing and sharing code.

### What Is Git ?

Git is a free and open-source distributed version control system. It allows developers to track changes to their code and collaborate with other developers on a project. With Git, you can keep a history of your code, revert to previous versions, and manage branches to experiment with new ideas.

### What is GitHub?

GitHub is a web-based platform that provides hosting for Git repositories. It makes it easy to share your code with others and collaborate on projects. GitHub provides a range of tools for project management, issue tracking, and collaboration, making it a popular platform for hosting open-source projects.

### Key Features of Git and GitHub

- **Distributed Version Control:** Git allows you to work with a local copy of your code, so you can work offline and avoid the need for a central server. This also makes it easy to backup your code and collaborate with others.
- **Branching and Merging:** With Git, you can create branches to experiment with new ideas, and then merge those changes back into the main codebase when you're ready.
- **Collaboration:** GitHub makes it easy to share your code with others and collaborate on projects. You can invite others to contribute, review changes, and track issues.
- **Issue Tracking:** GitHub provides a built-in issue tracking system, making it easy to manage bugs, features, and tasks for your project.

### How to Use Git and GitHub

1. Create a repository on GitHub
2. Clone the repository to your local machine
3. Make changes to the code
4. Stage and commit the changes using Git
5. Push the changes to the remote repository on GitHub
6. Collaborate with others by reviewing and merging changes

### Best Practices for Git and GitHub

- Write clear and concise commit messages
- Use branches for new features and bug fixes
- Keep your repository organized and avoid including unnecessary files
- Write a README file to provide information about your project
   
By using Git and GitHub, you can manage and share your code efficiently and effectively. Whether you're working on a small side project or a large open-source project, these tools will help you keep your code organized and make collaboration easier.

## Resources
### Read or Watch:

- [Resources To Learn Git](https://intranet.hbtn.io/rltoken/FsIQhm1yTLE3UZyOMwIClw)
- [Git And Github Cheat Sheet](https://intranet.hbtn.io/concepts/879)
- [The Framework](https://intranet.hbtn.io/concepts/880)
- [Approaching A Project](https://intranet.hbtn.io/concepts/881)

**Resources for advanced tasks** (Read only after finishing the mandatory tasks):

- [Learning Branching](https://intranet.hbtn.io/rltoken/wgk6wsgOUg6bIY1tjt6ehQ)
- [Good Practices For Teams Using Github](https://intranet.hbtn.io/rltoken/F6QfWb4HU1IgU4mwNEY1cA)

## Requirements

- A `README.md` file at the root of the repo, containing a description of the repository
- A `README.md` file, at the root of the folder of this project (i.e. git), describing what this project is about
- **Do not use GitHub’s web UI**, but the command line to perform the exercise (except for operations that can not possibly be done any other way than through the web UI). You won’t be able to perform many of the task requirements on the web UI, and you should start getting used to the command line for simple tasks because many complex tasks can only be done via the command line.
- Your answer files should only contain the command, and nothing else

## More Info
**Install** `git`

If `git` is not already installed on your terminal:
```
$ sudo apt-get update
$ sudo apt-get upgrade
$ sudo apt-get install git
```

**Basic usage**  

At the end of this project you should be able to reproduce and understand these command lines:
```
$ git clone <repo>
$ touch test
$ git add test
$ git commit -m "Initial commit"
$ git push origin main
```

----------------------------------

# Tasks

### [0. Create And Setup Your Git And Github Account](https://github.com/MathieuMorel62/holbertonschool-zero_day/tree/master/git)

**Step 0 - Create an account on GitHub**  

You will need a GitHub account for all your projects. You can create an account for free [here](https://intranet.hbtn.io/rltoken/-mliVC8UBjdpAGbt2IKWTQ)

**Step 1 - Create a Personal Access Token on Github**  

To have access to your repositories and authenticate yourself, you need to create a Personal Access Token on Github.

You can follow [this tutorial](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) to create a token.

**Step 2 - Update your profile on the Intranet**  

Update your Intranet profile by adding your Github username [here](https://intranet.hbtn.io/rltoken/FwTaZlU2qLyPNVwkKAnX9w)

If it’s not done the Checker won’t be able to correct your work

**Step 3 - Create your first repository**  

Using the graphic interface on the [github website](https://intranet.hbtn.io/rltoken/-mliVC8UBjdpAGbt2IKWTQ), create your first repository.

- Name: Look at the bottom of the project to see the name of the repository
- Description: `This is my first repository as a full-stack engineer`
- Public repo
- No `README`, `.gitignore`, or license

**Step 4 - Open the sandbox**  

On the intranet, just under the task, click on the button `>_Get a sandbox` and `run` to start the machine.
Once the container is started, click on `>_Webterm` to open a shell where you can start work from.

**Step 5 - Clone your repository**  

On the webterm of the sandbox, do the following:

- Clone your repository

```
root@896cf839cf9a:/# git clone https://{YOUR_PERSONAL_TOKEN}@github.com/{YOUR_USERNAME}/{YOUR_REPO}.git                  
Cloning into '{YOUR_REPO}'...
warning: You appear to have cloned an empty repository.
```

**Replace {YOUR_PERSONAL_TOKEN} with your token from step 1**  
**Replace {YOUR_USERNAME} with your username from step 0 and 1**  
**Replace {YOUR_REPO} with the name of the reposotiry at the bottom of the task**  

**Step 6 - Create the README.md and push the modifications**

- Navigate to this new directory. [Tips](https://askubuntu.com/questions/232442/how-do-i-navigate-between-directories-in-terminal)
```
root@896cf839cf9a:/# cd {YOUR_REPO}/
root@896cf839cf9a:/{YOUR_REPO}#
```

- Create the file `README.md` with the content `My first readme`. [Tips](https://forum.howtoforge.com/threads/echo-into-a-file.115/)
```
root@896cf839cf9a:/{YOUR_REPO}# echo 'My first readme' > README.md                                                                 
root@896cf839cf9a:/{YOUR_REPO}# cat README.md                                                                                      
My first readme                                                                                                                       
```

- Add this new file to git, commit the change with this message “My first commit” and push to the remote server / origin
```
root@896cf839cf9a:/{YOUR_REPO}# git add .
root@896cf839cf9a:/{YOUR_REPO}# git commit -m 'My first commit'
[master (root-commit) 98eef93] My first commit
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
root@896cf839cf9a:/{YOUR_REPO}# git push                                                                                           
Enumerating objects: 3, done.                                                                                                         
Counting objects: 100% (3/3), done.                                                                                                   
Writing objects: 100% (3/3), 212 bytes | 212.00 KiB/s, done.                                                                          
Total 3 (delta 0), reused 0 (delta 0)                                                                                                 
To https://github.com/{YOUR_USERNAME}/{YOUR_REPO}.git                                                                                       
 * [new branch]      master -> master 
 ```
 
 Good job!

You pushed your first file in your **first repository.**  
You can now check your repository on GitHub to see if everything is good.

--------------------------------

### [1. Repo-Session](https://github.com/MathieuMorel62/holbertonschool-zero_day/tree/master/git)

Create a new directory called `git` in your repo.  
Make sure you include a not empty `README.md` in your directory:
- at the root of your repository
- AND in the directory `git`

And important part: __Make sure your commit and push your code to Github - otherwise the Checker will always fail.__

----------------------------------

### [2. Coding Fury Road](https://github.com/MathieuMorel62/holbertonschool-zero_day/tree/master/git/c)

For the moment we have an empty project directory containing only a `README.md`. It’s time to code !

- Create these directories at the root of your project: `bash`, `c`, `js`
- Create these empty files:
  - `c/c_is_fun.c`
  - `js/main.js`
  - `js/index.js`
- Create a file `bash/best` with these two lines inside: `#!/bin/bash` and `echo "Best"`
- Create a file `bash/school` with these two lines inside: `#!/bin/bash` and `echo "School"`
- Add all these new files to git
- Commit your changes (message: “Starting to code today, so cool”) and push to the remote server

---------------------------------------

### [3. Collaboration Is The Base Of a Company](https://github.com/MathieuMorel62/holbertonschool-zero_day/tree/master/git/bash)

A branch is like a copy of your project. It’s used mainly for:  
- adding a feature in development
- collaborating on the same project with other developers
- not breaking your entire repository
- not upsetting your co-workers

The purpose of a branch is to isolate your work from the main code base of your project and/or from your co-workers’ work.

For this project, create a branch `update_script` and in this branch:
- Create an empty file named `bash/98`
- Update `bash/best` by replacing `echo "Best"` with `echo "Best School"`
- Update `bash/school` by replacing `echo "School"` with `echo "The school is open!"`
- Add and commit these changes (message: “My personal work”)
- Push this new branch [Tips](https://docs.github.com/en/get-started/using-git/pushing-commits-to-a-remote-repository)

Perfect! You did an amazing update in your project and it’s isolated correctly from the main branch.

Ho wait, your manager needs a quick fix in your project and it needs to be deployed now:
- Change branch to `main`
- Update the file `bash/best` by replacing `echo "Best"` with `echo "This School is so cool!"`
- Delete the directory `js`
- Commit your changes (message: “Hot fix”) and push to the origin
 
-----------------------------------

### [4. Collaboration: Be Up To Date](https://github.com/MathieuMorel62/holbertonschool-zero_day/blob/master/git/up_to_date)

Of course, you can also work on the same branch as your co-workers and it’s best if you keep up to date with their changes.  
 
For this task – **and only for this task** – please update your file `README.md` in the main branch from GitHub.com. It’s the **only time** you are allowed to update and commit from GitHub interface.

After you have done that, in your terminal:
- Get all changes of the main branch locally (i.e. your `README.md` file will be updated)
- Create a new file `up_to_date` at the root of your directory and in it, write the git command line used
- Add `up_to_date` to git, commit (message: “How to be up to date in git”), and push to the origin

----------------------------------

### [5. Haaa What Did You Do ???](https://github.com/MathieuMorel62/holbertonschool-zero_day/tree/master/git)

Collaboration is cool, but not really when you update the same file at the same time…

To illustrate that, please merge the branch `update_script` to `main`: “Cool, all my changes will be now part of the main branch, ready to be deployed!”

**HHHHHHHAAAAAAAA**
```
CONFLICT (content): Merge conflict in bash/best
```

As you can see, you have conflicts between two branches on the same file.

Your goal now is to resolve conflicts by using the version of the branch `update_script`, and push the result to the origin.

At the end, you should have all your work from the branch `update_script` (new file and two updated files) and all latest `main` commits (new files, delete folder, etc.), without conflicts.

-----------------------------------

### [6. Never Push Too Much](https://github.com/MathieuMorel62/holbertonschool-zero_day/blob/master/git/.gitignore)

Create a `.gitignore` file and define a rule to never push ~ files (generated by Emacs). [Tips](https://git-scm.com/docs/gitignore)

-------------------------------------

## AUTHOR

- Mathieu Morel
