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
	- Download GitHub CLI from: `https://www.cli.github.com`
	- Install the file prefixed with "gh".

## Configuring Github - machine
	- In your system's terminal, run  `gh auth login `
	- Follow the onscreen instructions for authenticating GitHub on your machine.

## Installing Git:
	- Download Git from: > git-scm.com
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
	- Start the ssh agent: `eval \`ssh-agent -s\``
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
	- Type `git commit -m ["Description of commit"]`
	- Type `git push origin master`

## Webstorm:
	Webstorm is an integrated development environment (IDE) designed for web development.
I personally will not be using Webstorm for my development. A student license copy of Webstorm 
can be downloaded for free from:
https://www.jetbrains.com/webstorm/download/

You may apply for a student license here:
https://www.jetbrains.com/community/education/#students

## Sources:
https://programmingwithswift.com/ssh-add-could-not-open-a-connection-to-your-authentication-agent/
https://jhooq.com/github-permission-denied-publickey/
https://github.github.com/gfm/#code-spans
https://kbroman.org/github_tutorial/pages/init.html
