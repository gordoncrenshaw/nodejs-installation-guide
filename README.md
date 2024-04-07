# Node.js Installation Guide

These instructions are for Mac OS using the zsh shell, which is the default shell.  

## Installation Instructions

1. Open Terminal window.
2. Type 'cd ~' and Enter.
3. Type 'ls -al' and Enter.
4. If the .zshrc file is missing, create the file by typing 'touch ~/.zshrc' and Enter.
5. Clone the nvm repository from Github.  Type 'git clone https://github.com/nvm-sh/nvm.git .nvm'
6. Open your ./zshrc configuration file.  Type 'vi .zshrc'
7. Add 'source ~/.nvm/nvm.sh' to the bottom of your file and save it.
8. Restart the terminal or source the ./zshrc file.  Type 'source ~/.zshrc'.
9. Verify nvm is installed.  Type 'nvm --version'.
10. Install the node.js.   Type 'nvm install node' to install the latest version of node.
11. Verify node.js and npm are installed.  Type 'node -v' and 'npm -v'.
12. To install a desired version of node, type 'nvm install v16.6.0'
13. To check the list of node versions we can use, type 'nvm ls'.
14. To swithc node.js versons, type 'nvm use v<version number>'.  For example 'nvm use v21.7.2'.

## Uninstall Instructions

1. Open Terminal window.
2. Type 'cd ~' and Enter.
3. To remove node.js using npm, type 'npm uninstall -g node' and Enter.
4. To remove the Node.js executable and the npm modules:
   
   a. Type 'sudo rm /usr/local/bin/node' and Enter.
   
   b. Type 'sudo rm -rf /usr/local/lib/node_modules' and Enter.
   
6. To remove the Node.js home directory, type 'rm -rf ~/.npm' and Enter.
7. To Remove the nvm installation directory, type 'rm -rf ~/.nvm' and Enter.
8. Remove the nvm script file from .zshrc:
   
   a. vi ~/.zshrc
   
   b. find and delete the line 'source ~/.nvm/nvm.sh'.
   
   c. Save and exit the vi editor.
   
10. Restart the terminal window.

Node.js, npm and nvm should be removed from your Mac. You can verify the uninstallation by running the following command:

  a. node -v
  
  b. npm -v
  
  c. nvm -v
  
If Node.js, npm and nvm are uninstalled, you should see an error message saying that the associated command is not found.
