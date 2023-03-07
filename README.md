# git-guide
This will show hot to setup a command line Git for Windows, the exact needed commands and steps to initlize that

Here are the steps to sign in to your GitHub account using a personal access token from Git Bash (Install if not exist) on Windows:

Open Git Bash on your Windows computer.

Use the following command to set your GitHub username:


    git config --global user.name "Your GitHub username"
    
Replace "Your GitHub username" with your actual GitHub username.

Use the following command to set your GitHub email address:

    git config --global user.email "Your GitHub email address"

Replace "Your GitHub email address" with the email address associated with your GitHub account.

Generate a personal access token from your GitHub account settings / Developer Settings / Personal Access Token.

In Git Bash, use the following command to set the token as your Git credential:

    git config --global credential.helper store

This command will store your credentials, including the personal access token, in a plain-text file on your computer. You can alternatively use a more secure credential helper, such as Git Credential Manager Core (GCM Core), which stores your credentials securely in the Windows Credential Manager.

Use the following command to sign in to your GitHub account using the personal access token:

    git clone https://github.com/username/repo.git

Replace "username" with your GitHub username and "repo" with the name of the repository you want to clone.

When prompted for a username and password, enter your GitHub username and the personal access token you generated in step 4, respectively.

Once you have successfully authenticated, you should be able to access your GitHub account from Git Bash using Git.

Note that the personal access token should be kept secure, and you should avoid sharing it with others. Also, be sure to replace "username" and "repo" in the command in step 6 with your actual GitHub username and repository name, respectively.
