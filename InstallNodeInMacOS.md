> We strongly recommend using a Node version manager like nvm to install Node.js and npm. We do not recommend using a Node installer, since the Node installation process installs npm in a directory with local permissions and can cause permissions errors when you run npm packages globally.

https://docs.npmjs.com/downloading-and-installing-node-js-and-npm

### Install NVM

More details can be read here:
https://github.com/nvm-sh/nvm

Run command to Install

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
```

If you use bash, the previous default shell, your system **may not have a .bash_profile file** where the command is set up. 
Create one with ```touch ~/.bash_profile``` and run the install script again. Then, run ```source ~/.bash_profile``` to pick up the nvm command.


#### Thoubleshooting - Git not working in MacOS

Git is not working after macOS Update (xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools)

https://stackoverflow.com/questions/52522565/git-is-not-working-after-macos-update-xcrun-error-invalid-active-developer-pa

The problem is that Xcode Command-line Tools needs to be updated.


Go back to your terminal and enter:

```
xcode-select --install
```

### Install Node

To download, compile, and install the latest release of node, do this:

```
nvm install node # "node" is an alias for the latest version

node -v
```

### Install NPM


you can at any time run the following command to get the latest supported npm version on the current node version:

```
nvm install-latest-npm
```
