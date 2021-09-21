My *Awesome* Readme  
Wesley Fegan  
IS117-005  
September 17, 2021  

#Using Git in conjunction with Github

## Configuring GitHub - web
- Navigate to https://www.github.com
- Create an account.
- Create a new repository.

## Installing GitHub
- Download GitHub CLI from: https://www.cli.github.com
- Install the file prefixed with "gh".

## Configuring Github - machine
- In your system's terminal, run `gh auth login`
- Follow the onscreen instructions for authenticating GitHub on your machine.

## Installing Git:
- Download Git from: git-scm.com
- Install Git

## Configuring Git:
- Set username and email to be the same as your GitHub account:
	`git config user.name "[GitHub Username]"`  
	`git config user.email "[GitHub Email]"`  

## Authenticating Your Machine With Github
- Open Bash (included with Git for Windows User).
- `cd ~/.ssh`
- `ssh-keygen`
- Give your SSH key an appropriate name
- Copy your public key into your clipboard:
	- Windows:  `cat key.pub | clip`
- Navigate to your account settings on the GitHub website and add your SSH key.
- Use the ssh-add command to add your private key.
- Start the ssh agent: ``eval `ssh-agent -s` ``
- Add your key: `ssh-add ~/.ssh/[private-key]`

You should now be ready to make commits to your repository.

## Making your first commit.
- Open the GitHub website in your browser and create a new repository.
- Create a folder on your local disk with a name that matches your repository's name.
- Navigate to the disk.
- Create some files.
- Type `git init`
- Type `git remote add origin git@github.com:[repository].git`
- Type `git add [Filename]` for each file in your folder.
- Type `git commit -m "[Description of commit]"`
- Type `git push origin master`

## Webstorm:
Webstorm is an integrated development environment (IDE) designed for web development.
I personally will not be using Webstorm for my development. A student license copy of Webstorm 
can be downloaded for free from:  
https://www.jetbrains.com/webstorm/download/
  
You may apply for a student license here:
https://www.jetbrains.com/community/education/#students  
  
Once installed, you will need to open the settings and navigate to version control section.
Here you will set your VC system as Git and provide the path to the Git executable.
  
For much more in depth instructions on configuring Webstorm, enabling Git, creating a project, and managing a repository from Webstorm please see "ExtraInstallationInstructions-20200214.pdf" from the IS117 Canvas page.  

## Glossary
- **Branch**: Version of a project or repository.
- **Clone**: Clone a repository into a new repository/directory (man7).
- **Commit**: Record changes to the repository (man7).
- **Fetch**: Download files from a repository (man7).
- **GIT**: "the stupid content tracker" (man7). Git is a revision control system, used primarily for code but is content agnostic.
- **Github**: Repository hosting service.
- **Merge**: Combine changes from multiple users (man7).
- **Merge Conflict**: Changes from multiple commits overlap eachother and Git cannot make sense of the changes.
- **Push**: Confirm and transmit local changes to the repository (man7).
- **Pull**: Retrieve content from a repository or branch (man7).
- **Remote**: Refers to a repository that is hosted on an external server.
- **Repository**: A location where a Git project's data is stored.

## Sources:
These are some helpful webpages I visited while configuring Git and Github:  
https://man7.org/linux/man-pages/man1/git.1.html  
https://programmingwithswift.com/ssh-add-could-not-open-a-connection-to-your-authentication-agent/  
https://jhooq.com/github-permission-denied-publickey/  
https://github.github.com/gfm/#code-spans  
https://kbroman.org/github_tutorial/pages/init.html  
