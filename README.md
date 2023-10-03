# OptimizeKit | Developer Environment Setup and Prerequisites for OptimizeKit


Overview

OptimizeKit is a set of coding recipes, developer guidelines, industry standard best practices and design patterns that supercharge workflows for software engineers and developers
Repo

The repo for OptimizeKit can be found below
GitHub - arunabhdas/OptimizeKit: OptimizeAI is a set of coding recipes, software industry standard…
OptimizeAI is a set of coding recipes, software industry standard best practices and design patterns that supercharge…

github.com
Change shell to bash (Optional, Recommended)

The default shell is zsh on mac. Changing it back to bash is recommended but not mandatory in order to follow along with the steps in this OptimizeDevKit

chsh -s /bin/bash
Install homebrew
Homebrew
The Missing Package Manager for macOS (or Linux).

brew.sh

/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

Setup SSH for Github

Ensure your SSH keys are correctly setup for Github

https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
Download and install AndroidStudio

https://developer.android.com/
Download and install Xcode

Xcode and related tools can be found here
Sign in with your Apple ID
Sign in with your Apple ID

Sign in with your Apple IDdeveloper.apple.com
Install Apple Developer Tools

Install Apple Developer Tools from here :
https://developer.apple.com/downloads/
Speed up Mouse Tracking on Mac OS X

http://www.tylernichols.com/apple/speed-up-mouse-tracking-on-mac-os-x
Install cocoapods and carthage

Install cocoapods as follows

sudo gem install cocoapods

Install carthage as follows

brew install cocoapods

Install nvm

https://github.com/creationix/nvm


curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.31.0/install.sh | bash

Add the following line in ~/.bashrc :

source ~/.nvm/nvm.sh
or
. ~/.nvm/nvm.sh
nvm install 16.20.0

Install the latest Node.js version

To install the latest available version of Node.js, you can use the following command:


nvm install node

Next, to use that version of Node.js in any new shell, you can simply run the use command:

nvm use node

Install node

brew install node

brew upgrade node

$ nvm install v6.0.0

Install Java Using SDKman

Install SDKman from https://sdkman.io

curl -s "https://get.sdkman.io" | bash

Install VSCode
Visual Studio Code - Code Editing. Redefined
Visual Studio Code is a code editor redefined and optimized for building and debugging modern web and cloud…

code.visualstudio.com

Install vim emulation for VSCode
https://github.com/VSCodeVim/Vim
Install SmoothMouse

http://smoothmouse.com/
Install python3

brew doctor

brew install python3

python3 - version

Add to PATH in .bash_profile or .bashrc
Configure Python3

source ~/.bash_profile

source ~/.bashrc

python3 - version

Create Virtual Python env as follows

python3 -m venv myvenv

source ~/myvenv/bin/activate

Check python version as follows

python -V

Python 3.4.3

Deactivate python env as follows


deactivate

Install Xcode Dev Tools

xcode-select -p

xcode-select - install

Install imagemagick

brew install imagemagick

Install gpg

brew install gpg

gpg2 - keyserver hkp://keys.gnupg.net - recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3

Install Ruby

The best way to install ruby on macOS is using rbenv
https://www.digitalocean.com/community/tutorials/how-to-install-ruby-on-rails-with-rbenv-on-macos
Install rails

Do not use system ruby —
https://thoughtbot.com/blog/psa-do-not-use-system-ruby
Install Bundler

sudo gem install bundler

Install Jekyll

https://www.taniarascia.com/make-a-static-website-with-jekyll/

jekyll new myjekyll
Brew install blade

https://github.com/jondot/blade

brew tap jondot/tap

brew install blade

Install IntelliJIdea

Install IntelliJIdea Community from

https://www.jetbrains.com/idea/?fromMenu#chooseYourEdition

Import settings from intellij-idea-community-settings folder
Install Google Cloud SDK

Install Cloud Tools version (156.0.0 at the time of authoring) from

http://cloud.google.com/sdk/docs/nstall the latest Cloud Tools version (156.0.0)
Install postgres

brew install postgresql
Install postgres from
http://postgresapp.com/

Install pgAdmin from
https://www.pgadmin.org/download/
Install mysql

Download and install mysql server from

https://dev.mysql.com/downloads/mysql/
Install Heroku CLI

Install Heroku CLI from steps
https://devcenter.heroku.com/articles/heroku-cli

brew tap heroku/brew && brew install heroku
Workaround for M1 Apple Silicon mac

First install homebrew for M1 chip:

~~~
arch -x86_64 /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
~~~
Then install the package on this new architecture:
~~~
arch -x86_64 brew install heroku
arch -arm64 brew install heroku
~~~
This solution works for every other brew package as well on M1 chip once you run the first step above:
~~~
arch -x86_64 brew install -package-name-
~~~

Install awswebcli (Optional)

Install EB CLI as follows

http://docs.aws.amazon.com/elasticbeanstalk/latest/dg/eb-cli3-install-osx.html
Install go (Optional)

brew install go
Install Charles proxy

https://www.charlesproxy.com/documentation/proxying/ssl-proxying/
Install Postman

Install Postman using

https://www.postman.com/downloads/
Install Stitch

Install Mono, Fiddler
https://www.telerik.com/download/fiddler-wizard
Install pushpin

Install and setup Pushpin
http://pushpin.org/
Install Dart

brew tap dart-lang/dart
brew install dart — with-content-shell — with-dartium
Setup Git completion

brew install git bash-completion

Install Python Toolchain | Poetry

Install Poetry

https://poetry.eustace.io/docs/
Install Python Toolchain | Streamlit

https://streamlit.io/
Install Jhipster

npm install -g generator-jhipster
Install mvn

brew update
brew install maven
export M2_HOME=/usr/local/Cellar/maven/3.6.2/libexec
export M2=${M2_HOME}/bin
export PATH=${PATH}:${M2_HOME}/bin

Install docker

Install docker for macOS
https://docs.docker.com/desktop/install/mac-install/
Install hyper (Optional)

Install hyper from here

https://hyper.is/
Install nativescript

Install nativescript CLI as described here

https://docs.nativescript.org/environment-setup.html
Install flutter

https://flutter.dev/docs/get-started/install/macos
Install anaconda

Install anaconda using brew

brew install - cask anaconda
…
PREFIX=/usr/local/anaconda3
…
Add to .bashrc -
# Anaconda path munging
export PATH=${PATH}:/usr/local/anaconda3/bin
~~~
Run
~~~
jupyter notebook

Install Pytorch

https://pytorch.org/get-started/locally/
Install Flutter

https://docs.flutter.dev/get-started/install/macos
Install Adobe

Install Adobe Creative Cloud
Install pnpm


npm install -g pnpm
