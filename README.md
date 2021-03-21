# pset-codes
PSET learns R, stats, and coding!

This is the onboarding guide - things to install and set up.

## Git
Git is a method of version control, meaning that it allows multiple contributers to add to work on the same project. We will be using GitHub kind of like Google Drive to document our progress. The code is stored in a repository (pset-codes). We each have a folder that contains our notes. Using git, we can see each other's notebooks. If and when we work on projects together (or you work on code with anyone else in your future), git is critical to ensuring a smooth workflow.
You can download the appropriate version of git here:
https://git-scm.com/book/en/v2/Getting-Started-Installing-Git

Next, make an account on GitHub, and ask Nidhi to be added as a collaborator to this repository.

## R
R is a statistical programming language. It is free and open source, and many psychologists (and other scientists) use R to conduct their statistical analsyses.
You can download the right version of R here:
https://cran.r-project.org/

## Anaconda
Anaconda is a Python installation that includes Jupyter notebook and R Studio. You can install Anaconda here: https://docs.anaconda.com/anaconda/install/

Python is a versatile and popular programming language that is used for practically everything. The package PsychoPy (https://www.psychopy.org/) allows you to create experiments, like the Stroop task.

Jupter notebook is where we will be documenting what we learn. A notebook is a file that consists of cells. The cells can be Markdown (like this document) or code (R in our case). Using these notebooks, we can write notes about what we learn and also include the code itself. These documents are really polished and are made to be shared and presented. Here's an example: https://hub.gke2.mybinder.org/user/binder-examples-r-jpbnriyj/notebooks/index.ipynb

R Studio is an integrated development environment (IDE) for R. It provides a workspace and many tools for running R scripts. R Studio also has an R Markdown notebook option that's kind of like Jupyter notebook.

## R Environment in Jupyter Notebook
Jupyter usually uses the Python kernel (the code is Python), so we have to create an R environment in Anaconda to use Jupyter with. Here are the instructions: https://docs.anaconda.com/anaconda/navigator/tutorials/r-lang/

## Jupyter Book
Optional: We don't really need this, but Jupyter Book allows us to bundle our notebooks into a pretty book that is hyperlinked, with navigation tabs, etc (kind of like most of the documentation links on this page). An example and instructions to get started can be found here: https://jupyterbook.org/intro.html

## Test Run
First, we need to set up the credentials for git (https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup). Go to the command prompt/terminal, and type the following lines into the command line (without the dollar signs, replaced with your information). Your user.name doesn't have to be the same as your GitHub username.
$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com
You can check your username by typing "git config user.name" and hitting enter.

Now, we are going to clone the pset-codes repository onto your local machine. First, figure out in what folder your want to store this code (like Desktop or Documents). Then, we will navigate to this folder in the command prompt. When you open the command prompt, it tells you what directory (folder) you are currently in. You can use the command "cd FolderName" to move into a subfolder of the one you are currerntly in, named FolderName. You can use "cd .." to move to the parent folder of the one you are currently in. Using these commands, navigate to the folder you want to house the code in.

To clone the repository, type in "git clone address" and replace "address" with the clone address of the repository (in this case, https://github.com/nidhipai/pset-codes.git). Now, if you open File Explorer, you should be able to see the folders that are on this repository. Create your own folder.

Open the R environment in Jupyter Notebook. It will show a file explorer; navigate to your folder inside the pset-codes folder. Inside that folder, click "New" and then "R". This will create a new notebook - you can rename it something like "First Notebook". Try typing some R code, such as "x <- 2 + 2" and "x" on the next line. Hit Shift+Enter to run the code and see the output. You can also try experimenting with Markdown.

Finally, we want to push our changes to GitHub so that everyone can access your code. It's a good habit to always pull other people's changes before you push. To pull other people's changes from GitHub, first, navigate inside the pset-codes folder in the terminal/command prompt. Then run "git pull". It will probably say "Already up to date." because it is unlikely anyboy pushed their changes since the time you cloned the repository. Now, we add the files you created with "git add ." . The dot stands for "all". This will allow git to track these files. We next commit our changes with "git commit -m "message". Replace message with something like "your name first commit". Then we push with "git push origin main". Sometimes it's "master" and sometimes it's the new "main", so if one doesn't work try the other.

## Helpful guides:
- R textbook: https://r4ds.had.co.nz/index.html
- Markdown cheat sheet: https://www.markdownguide.org/basic-syntax/
- Git cheat sheet: https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet
