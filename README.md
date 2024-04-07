# Node.js Installation Guide

These instructions are for Mac OS using the zsh shell, which is the default shell.  

## Installation Instructions

1. Open Terminal window, and execute `cd ~`.
2. Execute `ls -al`.
3. If the .zshrc file is missing, create the file by executing `touch ~/.zshrc`.
4. Clone the nvm repository from Github.  Type `git clone https://github.com/nvm-sh/nvm.git .nvm`.
5. Open your ./zshrc configuration file.  Type `vi .zshrc`.
6. Add `source ~/.nvm/nvm.sh` to the bottom of your file and save it.
7. Restart the terminal, or source the ./zshrc file by executing `source ~/.zshrc`.
8. Verify nvm is installed, by executing `nvm --version`.
9. Install the node.js.   Execute `nvm install node` to install the latest version of node.
10. Verify node.js and npm are installed.  Execute `node -v`, and execute `npm -v`.
11. To install a desired version of node, execute `nvm install v16.6.0`.
12. To check the list of node versions we can use, execute `nvm ls`.
13. To switch node.js versons, execute `nvm use v<version number>`; for example `nvm use v21.7.2`.

## Uninstall Instructions

1. Open Terminal window, and execute `cd ~`.
2. To remove node.js using npm, execute `npm uninstall -g node`.
3. To remove the Node.js executable and the npm modules:
   * Execute `sudo rm /usr/local/bin/node`.
   * Execute `sudo rm -rf /usr/local/lib/node_modules`.
5. To remove the Node.js home directory, execute `rm -rf ~/.npm`.
6. To Remove the nvm installation directory, execute `rm -rf ~/.nvm`.
7. Remove the nvm script file from .zshrc:
   * Execute `vi ~/.zshrc`.
   * find and delete the line `source ~/.nvm/nvm.sh`.
   * Save and exit the vi editor.
8. Restart the terminal window.

Node.js, npm and nvm should be removed from your Mac. You can verify the uninstallation by running the following commands:

* `node -v`
* `npm -v`
* `nvm -v`

If Node.js, npm and nvm are uninstalled, you should see an error message saying that the associated command is not found.
