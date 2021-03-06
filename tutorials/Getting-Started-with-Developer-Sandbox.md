

## Getting Started with Developer Sandbox ##
The installation walkthrough below will refer to Ubuntu, but you are free to use any other distribution. Depending on which you go for, the installation and package management instructions change, so keep that in mind when using something like Fedora, CentOS, or Arch.

#### References ####
  - https://code.tutsplus.com/tutorials/a-linux-developers-setup--cms-22138

  A common practice on agile teams is to ensure that developers have their own **"sandboxes"** to work in.
  > A sandbox is basically a technical environment whose scope is well defined and respected.
  >   
  > The primary advantage of sandboxes are that they help to reduce the risk of technical errors adversely affecting a larger group of people than is absolutely necessary at the time.

  This is the working environment of individual developers, programming pairs, or individual feature teams.

  The purpose of this environment is for the developer/pair/team to work in seclusion from the rest of their project team, enabling them to make and validate changes without having to worry about adversely affecting the rest of their project team.

  These environments are likely to have their own databases to enable regression testing and more importantly agile testing strategies.


## Step by Step Tutorial

#### Login ####
Using your user name and password login to the Ubuntu Desktop.

![Ubuntu Desktop image](images/sandbox-1.jpg)

#### Open terminal
Move mouse over search bard
![Ubuntu Desktop image](images/sandbox-2.jpg)

Type in "terminal" and select one of the terminial applications.
![Ubuntu Desktop image](images/sandbox-3.jpg)

#### Checks out System ####
Once you have the terminal running execute the following commands
> $ pwd    # where am i
>
> $ ls     # what i in current directory
>
> $ id     # who am I logged in as

![Ubuntu Desktop image](images/sandbox-4.jpg)

Now is time to install some prerequistes


#### Install the following prerequisites ####
Verify you have the following commands installed
- wget
- unzip
- curl
- git
- java


![image should be here](images/sandbox-5
.jpg)

For example to install git, check to see if **git is installed**. If not
> $git
>
> $ sudo apt install git
>
> $ git    # command should now be available


### JavaScript Developer Setup ###
Working with JavaScript is usually very easy to get started with, due to browsers being an active development asset. However, that's not the case in the server side. Node.js is available in most Linux distributions but the latest version is not always ready to be installed. For that purpose we'll install a Node version manager, install a version, and go from there.

The version manager that we'll use for this article is nvm, but you can also look up n as an alternative. If you go through the README you will need to paste the first instruction into a terminal:

1
$ curl https://raw.githubusercontent.com/creationix/nvm/v0.15.0/install.sh | bash
If you don't have curl installed, the command will complain. Type sudo apt-get install curl in your terminal, and then run the previous command again.

The command retrieves a script from GitHub that is run directly on your system. You will have nvm installed in your home folder so you won't have any trouble with permissions, unlike when you install it from the Ubuntu packages. You can check if nvm is correctly working by typing nvm in the terminal. If an error occurs, probably you'll need to edit your shell configuration file. Edit the .bashrc file as we did for chruby, and add the following code at the end of the file:
