# Getting started with Phaser 3 Tutorial
Link to tutorial: https://phaser.io/tutorials/getting-started-phaser3/index

1. Install NodeJS, Python, XAMP, WAMP or MAMP (essentially a webserver)
2. Install http-server (optional)
3. Install Phaser 3 (optional)
5. Run webserver

# Clone this repository
In your terminal of choice run the following commands:
```sh
mkdir -p ~/projects; cd ~/projects
git clone https://github.com/trungisme/getting-started-with-phaser3.git
cd getting-started-with-phaser3
```

# Installing NodeJS
For this tutorial, we will be using Ubuntu/Debian's apt package manager
Let's start by updating the linux packages
```sh
sudo apt-get update -y
sudo apt-get upgrade -y
```

We also need to install some basic build tool for node-gyp - node binaries build tool:
```sh
sudo apt-get install build-essential -y
```

We will install NPM using NVM (node version manager) due to its flexibility to manage and allow different versions of NPM:
```sh
# This command install version 0.35.0, check the NVM reference it there are newer versions.
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.0/install.sh | bash
```

Restart your terminal once the script has been executed.
We can now install the LTS (long term support) version for Node:
```sh
nvm install --lts
```

In order to use this version of node, we then run the following upon each instance of the terminal:
```sh
nvm use --lts
```
Or, alternatively, we can add it to our ~/.bashrc or ~/.bash_profile
```sh
echo "nvm use --lts" >> .bash_profile
```

You can now verify your version of node, npm and npx using the following:
(At the time of this tutorial the following versions were applicable.)
```sh
node -v #v12.16.1
npm -v #6.13.4
npx -v #6.13.4
```

# Installing http-server for npm
Link to guide used for reference: https://www.npmjs.com/package/http-server
Navigate to your repository location and install http-server
```sh
cd ~/projects/getting-started-with-phaser3
npm install -g http-server
```
You can now run the following command to start your webserver:
```sh
http-server .
```

Optionally, run http-server on demand
```sh
npx http-server .
```

# Installing Phaser 3
```sh
cd ~/projects/getting-started-with-phaser3
npm install phaser@3.22.0
```

# Run your webserver
As mentioned previously, you can run your webserver using httpserver or npx httpserver
```sh
npx httpserver .
```
