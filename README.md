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
	- Download GitHub CLI from: > https://www.cli.github.com
	- Install the file prefixed with "gh".

## Configuring Github - machine
	- In your system's terminal, run > gh auth login 
	- Follow the onscreen instructions for authenticating GitHub on your machine.

## Installing Git:
	- Download Git from: > git-scm.com
	- Install Git

## Configuring Git:
	- Set username and email to be the same as your GitHub account:
		> git config user.name "[GitHub Username]"
		> git config user.email "[GitHub Email]"

## Authenticating Your Machine With Github
	- Open Bash (included with Git for Windows User).
	- > cd ~/.ssh
	- > ssh-keygen
	- Give your SSH key an appropriate name
	- Copy your public key into your clipboard:
		- Windows: > cat key.pub | clip
	- Navigate to your account settings on the GitHub website and add your SSH key.
	- Use the ssh-add command to add your private key.

You should now be ready to make commits to your repository.
