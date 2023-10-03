# Developer Environment Setup and Prerequisites for OptimizeAI


### 0) Change shell to bash

chsh -s /bin/bash

### 0.1) Install brew

https://brew.sh

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### 0.2) Setup SSH for Bitbucket and Github

https://support.atlassian.com/bitbucket-cloud/docs/set-up-personal-ssh-keys-on-macos/

https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent

https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account?tool=webui

### 0.3) Clone projectdocs

### 0.4) Download and install AndroidStudio

### 0.5) Download and install Xcode

### 1) Chrome

Install Chrome

### 2) Apple Developer Tools 

Install Apple Developer Tools from here :
https://developer.apple.com/downloads/

### 3) Speed up Mouse Tracking on Mac OS X using instructions here :

http://www.tylernichols.com/apple/speed-up-mouse-tracking-on-mac-os-x


### 4) Subl shortcut 

Install sublime from here :

https://www.sublimetext.com/3

Add subl shortcut using the instructions here :

http://olivierlacan.com/posts/launch-sublime-text-3-from-the-command-line/


### 5) Vintageous

Install Vintageous for vi mode in sublime :

https://github.com/guillermooo/Vintageous#vintageous


### 6) ST3 PackageControl 

Install ST3 package control using instructions here :

https://packagecontrol.io/installation

https://packagecontrol.io/packages/Seti_UI

Also checkout instructions here for more info :

https://scotch.io/bar-talk/the-complete-visual-guide-to-sublime-text-3-getting-started-and-keyboard-shortcuts

### 7) Seti_UI

Install Seti_UI using package control :

https://packagecontrol.io/packages/Seti_UI

Cmd-Shift-P for invoking package control

### 8) Activate Seti_UI 

Activate the Seti_UI theme by modifying the user preferences file with the following entry :

{
    "theme": "Seti.sublime-theme"
}

as described in the setup instructions here :

https://packagecontrol.io/packages/Seti_UI

### 9) Twighlight theme

Download and install Twighlight theme :

https://github.com/biasedbit/xcode-themes

### 10) Alcatraz 

Install Alcatraz using steps here :

http://alcatraz.io/

### 11) XVim

Install Xvim using steps here :

https://github.com/XVimProject/XVim

To make XVim, first ensure that the path to command line tools is correct as described here :

https://github.com/XVimProject/XVim/issues/920 

$ sudo xcode-select -s ~/Developer/Xcode/Xcode_7_3/Xcode_7_3.app/Contents/Developer

$ xcode-select -p

/Users/das/Developer/Xcode/Xcode_7_3/Xcode_7_3.app/Contents/Developer

### 12) xvimrc 

Copy xvimrc to ~/.xvimrc and restart Xcode


### 13) Install cocoapods and carthage

Install cocoapods as follows :

$ sudo gem install cocoapods


Install carthage as follows :

$ brew install cocoapods

### 14) Disable ApplePressAndHold 

Disable ApplePressAndHold for ST3 as described here :

https://gist.github.com/kconragan/2510186

defaults write -g ApplePressAndHoldEnabled -bool false


### 15) Install Homebrew as described here :

http://brew.sh/

/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

### 16) Install nvm

https://github.com/creationix/nvm

curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.31.0/install.sh | bash

Add the following line in ~/.bashrc : 

source ~/.nvm/nvm.sh

or 

. ~/.nvm/nvm.sh

nvm install 16.20.0

~~~
Install the latest Node.js version
To install the latest available version of Node.js, you can use the following command:

nvm install node
Next, to use that version of Node.js in any new shell, you can simply run the use command:

nvm use node
~~~

### 17) Install node

~~~
$ brew install node

$ brew upgrade node
~~~

OR

~~~
$ nvm install v6.0.0
~~~
### 18) Install Cordova toolchain as described here :

http://cordova.apache.org/

$ npm install -g yeoman bower grunt-cli gulp cordova

$ sudo gem install compass

$ brew install graphicsmagick

#### Cordova [docs](https://cordova.apache.org/) `npm install cordova -g`

#### Android SDK: [Download](http://developer.android.com/sdk/installing/index.html)

#### Xcode command line tools: [Download](https://developer.apple.com/xcode/download/) or `xcode-select --install`

#### JAVA SDK (latest): [Download](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)


### 19) Install legacy Java from here 

https://support.apple.com/kb/DL1572?locale=en_US

or

https://support.apple.com/kb/DL1572?locale=en_US


### 20) Install Sublime snippets for ST3 at this location :

~/Library/Application\ Support/Sublime\ Text\ 3/Packages/User/(star).sublime-snippet

### 21) Install Atom editor

https://atom.io/

### 22) Install atom snippets at this location 

~/.atom/snippets.cson

### 23) Install atom packages as shown in screenshots/screenshot_1.png

![alt text](https://github.com/arunabhdas/mac-environment-setup/blob/master/screenshots/screenshot_1.png "Screenshot 1")

### 24) Install SmoothMouse

http://smoothmouse.com/


### 25) Install Android Studio

https://developer.android.com/studio/install.html


### 26) Install python3

~~~~
==> brew doctor
~~~~

~~~~
==> brew install python3

==> python3 --version
~~~~


Add to PATH in .bash_profile or .bashrc 

# Python 3 
export PATH="$HOME/.local/bin:$PATH"

source ~/.bash_profile 

or

source ~/.bashrc

Check version as follows

python3 -V

Create Virtual Python env as follows 
~~~~
==> sudo easy_install pip
~~~~

~~~~
==> sudo pip install --upgrade virtualenv
~~~~


~~~~
source ~/venv/bin/activate
~~~~

~~~~
mkdir ~/venv	
 virtualenv ~/venv
~~~~

Check python version as follows

~~~~
python -V
Python 3.4.3
~~~~

Exit python env as follows

~~~~
deactivate
~~~~

### 28) Install Java SE 6 Runtime from here :

https://support.apple.com/kb/DL1572?locale=en_US

### 29) Select the correct version of xcode tools as follows 

First check your current version of Xcode tools as follows :

==> xcode-select -p
/Users/das/Developer/Xcode/Xcode_7_3/Xcode_7_3.app/Contents/Developer

xcode-select --install

==> sudo xcode-select --switch /Users/coder/Developer/Xcode/Xcode_8_2_1/Xcode_8_2_1.app/Contents/Developer

==> xcode-select -p
/Users/coder/Developer/Xcode/Xcode_8_2_1/Xcode_8_2_1.app/Contents/Develope

### 30) Setup for Xvim for Xcode8 as documented here :

https://github.com/XVimProject/XVim/blob/master/INSTALL_Xcode8.md

and

http://zmoson.com/turn-xcode-into-vim-like-editor/

### 31) Build Xvim as documented here :

https://github.com/XVimProject/XVim


### 32) Install composer as follows :

curl -sS https://getcomposer.org/installer | php

sudo mv composer.phar /usr/local/bin

Add the following alias to .bashrc

alias composer="php /usr/local/bin/composer"

Add to path by adding the following to .bashrc / .bash_profile

export PATH=$PATH:$HOME/.composer/vendor/bin

### 33) Install the Laravel installer using Composer

composer global require "laravel/installer"

### 34) Add $HOME/.composer/vendor/bin to your $PATH


### 35) Install imagemagick

brew install imagemagick

### 36) Install gpg

brew install gpg

### 37) gpg2 --keyserver

gpg2 --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3


### 38)  Uninstall rvm 
Uninstall rvm and install rbenv and use it to install ruby as described here -

https://github.com/arunabhdas/mac-environment-setup/blob/master/STARTHERE.md


### 39) Check if Ruby is already installed as follows

==> rvm list rubies

==> bundle env

## The Best Way To Install Ruby
https://www.digitalocean.com/community/tutorials/how-to-install-ruby-on-rails-with-rbenv-on-macos

### The StackOverflow Way 

https://stackoverflow.com/questions/51664716/you-dont-have-write-permissions-for-the-library-ruby-gems-2-3-0-directory/54874320

As previously noted, on a Mac the system ruby is owned by root and it's not safe to install things against that version with sudo. If you do every gem runs as root and that's a security nightmare. DO NOT DO THAT

I'll walk you through my steps since previous answers assume a bit of command line foo and the added details might be of some use to someone.

Double-check we're running the old, system provided ruby

```
which ruby
/usr/bin/ruby
(that's the system path)

ruby -v
ruby 2.3.7
(the old version)

brew install ruby
or install brew first

at the end of which, the install says:

/usr/local/Cellar/ruby/2.6.3
Make that show up in the path first

PATH=/usr/local/Cellar/ruby/2.6.3/bin:$PATH
Double-check

which ruby
/usr/local/Cellar/ruby/2.6.3/bin/ruby
Double-check version

ruby --version
ruby 2.6.3p62
Make the path update permanent (otherwise you'll have to update the path each time you want to use ruby)

echo  PATH=/usr/local/Cellar/ruby/2.6.3/bin:$PATH >> ~/.bash_profile
```


### 40) Install rails :

Do not use system ruby - 
https://thoughtbot.com/blog/psa-do-not-use-system-ruby

~~~
==> ruby -v
ruby 2.6.3p62 (2019-04-16 revision 67580) [universal.x86_64-darwin19]
~/repos/appliaison/bitbucketrepos/wish-list-app/wish-list-app-rails6-backend (master) 

==> rvm list
=* ruby-2.7.0 [ x86_64 ]

# => - current
# =* - current && default
#  * - default



==> gem list

*** LOCAL GEMS ***

activesupport (4.2.11.1)
algoliasearch (1.27.1)
atomos (0.1.3)
bigdecimal (default: 1.4.1)
bundler (default: 1.17.2)
CFPropertyList (2.3.6)
claide (1.0.3)
cmath (default: 1.0.0)
cocoapods (1.8.4)
cocoapods-clean (0.0.1)
cocoapods-core (1.8.4)
cocoapods-deintegrate (1.0.4)
cocoapods-downloader (1.2.2)
cocoapods-plugins (1.0.0)
cocoapods-search (1.0.0)
cocoapods-stats (1.1.0)
cocoapods-trunk (1.4.1)
cocoapods-try (1.1.0)
colored2 (3.1.2)
concurrent-ruby (1.1.5)
csv (default: 3.0.9)
date (default: 2.0.0)
dbm (default: 1.0.0)
did_you_mean (1.3.0)
e2mmap (default: 0.1.0)
escape (0.0.4)
etc (default: 1.0.1)
fcntl (default: 1.0.0)
fiddle (default: 1.0.0)
fileutils (default: 1.1.0)
forwardable (default: 1.2.0)
fourflusher (2.3.1)
fuzzy_match (2.0.4)
gh_inspector (1.1.3)
httpclient (2.8.3)
i18n (0.9.5)
io-console (default: 0.4.7)
ipaddr (default: 1.2.2)
irb (default: 1.0.0)
json (default: 2.1.0)
libxml-ruby (3.1.0)
logger (default: 1.3.0)
matrix (default: 0.1.0)
mini_portile2 (2.4.0)
minitest (5.11.3)
molinillo (0.6.6)
mutex_m (default: 0.1.0)
nanaimo (0.2.6)
nap (1.1.0)
net-telnet (0.2.0)
netrc (0.11.0)
nokogiri (1.10.1)
openssl (default: 2.1.2)
ostruct (default: 0.1.0)
power_assert (1.1.3)
prime (default: 0.1.0)
psych (default: 3.1.0)
rake (12.3.2)
rdoc (default: 6.1.0)
rexml (default: 3.1.9)
rss (default: 0.2.7)
ruby-macho (1.4.0)
scanf (default: 1.0.0)
sdbm (default: 1.0.0)
shell (default: 0.7)
sqlite3 (1.3.13)
stringio (default: 0.0.2)
strscan (default: 1.0.0)
sync (default: 0.5.0)
test-unit (3.2.9)
thread_safe (0.3.6)
thwait (default: 0.1.0)
tracer (default: 0.1.0)
tzinfo (1.2.5)
webrick (default: 1.4.2)
xcodeproj (1.13.0)
xmlrpc (0.3.0)
zlib (default: 1.0.0)


==> ruby -v
ruby 2.6.3p62 (2019-04-16 revision 67580) [universal.x86_64-darwin19]
~/repos/appliaison/bitbucketrepos/wish-list-app/wish-list-app-rails6-backend (master) 
==> gem -v
3.0.3


==> rails -v
Rails is not currently installed on this system. To get the latest version, simply type:

    $ sudo gem install rails

You can then rerun your "rails" command.
~/repos/appliaison/bitbucketrepos/wish-list-app/wish-list-app-rails6-backend (master) 
==> sudo gem install rails
Password:
Fetching zeitwerk-2.4.0.gem
Fetching rack-2.2.3.gem
Fetching activesupport-6.0.3.2.gem
Fetching rack-test-1.1.0.gem
Fetching crass-1.0.6.gem
Fetching loofah-2.6.0.gem
Fetching rails-html-sanitizer-1.3.0.gem
Fetching rails-dom-testing-2.0.3.gem
Fetching builder-3.2.4.gem
Fetching erubi-1.9.0.gem
Fetching actionview-6.0.3.2.gem
Fetching actionpack-6.0.3.2.gem
Fetching activemodel-6.0.3.2.gem
Fetching activerecord-6.0.3.2.gem
Fetching globalid-0.4.2.gem
Fetching activejob-6.0.3.2.gem
Fetching mini_mime-1.0.2.gem
Fetching mail-2.7.1.gem
Fetching actionmailer-6.0.3.2.gem
Fetching nio4r-2.5.2.gem
Fetching websocket-extensions-0.1.5.gem
Fetching websocket-driver-0.7.3.gem
Fetching actioncable-6.0.3.2.gem
Fetching mimemagic-0.3.5.gem
Fetching marcel-0.3.3.gem
Fetching activestorage-6.0.3.2.gem
Fetching actionmailbox-6.0.3.2.gem
Fetching actiontext-6.0.3.2.gem
Fetching thor-1.0.1.gem
Fetching method_source-1.0.0.gem
Fetching railties-6.0.3.2.gem
Fetching sprockets-4.0.2.gem
Fetching sprockets-rails-3.2.1.gem
Fetching rails-6.0.3.2.gem
Successfully installed zeitwerk-2.4.0
Successfully installed activesupport-6.0.3.2
Successfully installed rack-2.2.3
Successfully installed rack-test-1.1.0
Successfully installed crass-1.0.6
Successfully installed loofah-2.6.0
Successfully installed rails-html-sanitizer-1.3.0
Successfully installed rails-dom-testing-2.0.3
Successfully installed builder-3.2.4
Successfully installed erubi-1.9.0
Successfully installed actionview-6.0.3.2
Successfully installed actionpack-6.0.3.2
Successfully installed activemodel-6.0.3.2
Successfully installed activerecord-6.0.3.2
Successfully installed globalid-0.4.2
Successfully installed activejob-6.0.3.2
Successfully installed mini_mime-1.0.2
Successfully installed mail-2.7.1
Successfully installed actionmailer-6.0.3.2
Building native extensions. This could take a while...
Successfully installed nio4r-2.5.2
Successfully installed websocket-extensions-0.1.5
Building native extensions. This could take a while...
Successfully installed websocket-driver-0.7.3
Successfully installed actioncable-6.0.3.2
Successfully installed mimemagic-0.3.5
Successfully installed marcel-0.3.3
Successfully installed activestorage-6.0.3.2
Successfully installed actionmailbox-6.0.3.2
Successfully installed actiontext-6.0.3.2
Successfully installed thor-1.0.1
Successfully installed method_source-1.0.0
Successfully installed railties-6.0.3.2
Successfully installed sprockets-4.0.2
Successfully installed sprockets-rails-3.2.1
Successfully installed rails-6.0.3.2
Parsing documentation for zeitwerk-2.4.0
Installing ri documentation for zeitwerk-2.4.0
Parsing documentation for activesupport-6.0.3.2
Installing ri documentation for activesupport-6.0.3.2
Parsing documentation for rack-2.2.3
Installing ri documentation for rack-2.2.3
Parsing documentation for rack-test-1.1.0
Installing ri documentation for rack-test-1.1.0
Parsing documentation for crass-1.0.6
Installing ri documentation for crass-1.0.6
Parsing documentation for loofah-2.6.0
Installing ri documentation for loofah-2.6.0
Parsing documentation for rails-html-sanitizer-1.3.0
Installing ri documentation for rails-html-sanitizer-1.3.0
Parsing documentation for rails-dom-testing-2.0.3
Installing ri documentation for rails-dom-testing-2.0.3
Parsing documentation for builder-3.2.4
Installing ri documentation for builder-3.2.4
Parsing documentation for erubi-1.9.0
Installing ri documentation for erubi-1.9.0
Parsing documentation for actionview-6.0.3.2
Installing ri documentation for actionview-6.0.3.2
Parsing documentation for actionpack-6.0.3.2
Installing ri documentation for actionpack-6.0.3.2
Parsing documentation for activemodel-6.0.3.2
Installing ri documentation for activemodel-6.0.3.2
Parsing documentation for activerecord-6.0.3.2
Installing ri documentation for activerecord-6.0.3.2
Parsing documentation for globalid-0.4.2
Installing ri documentation for globalid-0.4.2
Parsing documentation for activejob-6.0.3.2
Installing ri documentation for activejob-6.0.3.2
Parsing documentation for mini_mime-1.0.2
Installing ri documentation for mini_mime-1.0.2
Parsing documentation for mail-2.7.1
Installing ri documentation for mail-2.7.1
Parsing documentation for actionmailer-6.0.3.2
Installing ri documentation for actionmailer-6.0.3.2
Parsing documentation for nio4r-2.5.2
Installing ri documentation for nio4r-2.5.2
Parsing documentation for websocket-extensions-0.1.5
Installing ri documentation for websocket-extensions-0.1.5
Parsing documentation for websocket-driver-0.7.3
Installing ri documentation for websocket-driver-0.7.3
Parsing documentation for actioncable-6.0.3.2
Installing ri documentation for actioncable-6.0.3.2
Parsing documentation for mimemagic-0.3.5
Installing ri documentation for mimemagic-0.3.5
Parsing documentation for marcel-0.3.3
Installing ri documentation for marcel-0.3.3
Parsing documentation for activestorage-6.0.3.2
Installing ri documentation for activestorage-6.0.3.2
Parsing documentation for actionmailbox-6.0.3.2
Installing ri documentation for actionmailbox-6.0.3.2
Parsing documentation for actiontext-6.0.3.2
Installing ri documentation for actiontext-6.0.3.2
Parsing documentation for thor-1.0.1
Installing ri documentation for thor-1.0.1
Parsing documentation for method_source-1.0.0
Installing ri documentation for method_source-1.0.0
Parsing documentation for railties-6.0.3.2
Installing ri documentation for railties-6.0.3.2
Parsing documentation for sprockets-4.0.2
Installing ri documentation for sprockets-4.0.2
Parsing documentation for sprockets-rails-3.2.1
Installing ri documentation for sprockets-rails-3.2.1
Parsing documentation for rails-6.0.3.2
Installing ri documentation for rails-6.0.3.2
Done installing documentation for zeitwerk, activesupport, rack, rack-test, crass, loofah, rails-html-sanitizer, rails-dom-testing, builder, erubi, actionview, actionpack, activemodel, activerecord, globalid, activejob, mini_mime, mail, actionmailer, nio4r, websocket-extensions, websocket-driver, actioncable, mimemagic, marcel, activestorage, actionmailbox, actiontext, thor, method_source, railties, sprockets, sprockets-rails, rails after 30 seconds
34 gems installed
~/repos/appliaison/bitbucketrepos/wish-list-app/wish-list-app-rails6-backend (master) 
==> gem list

*** LOCAL GEMS ***

actioncable (6.0.3.2)
actionmailbox (6.0.3.2)
actionmailer (6.0.3.2)
actionpack (6.0.3.2)
actiontext (6.0.3.2)
actionview (6.0.3.2)
activejob (6.0.3.2)
activemodel (6.0.3.2)
activerecord (6.0.3.2)
activestorage (6.0.3.2)
activesupport (6.0.3.2, 4.2.11.1)
algoliasearch (1.27.1)
atomos (0.1.3)
bigdecimal (default: 1.4.1)
builder (3.2.4)
bundler (default: 1.17.2)
CFPropertyList (2.3.6)
claide (1.0.3)
cmath (default: 1.0.0)
cocoapods (1.8.4)
cocoapods-clean (0.0.1)
cocoapods-core (1.8.4)
cocoapods-deintegrate (1.0.4)
cocoapods-downloader (1.2.2)
cocoapods-plugins (1.0.0)
cocoapods-search (1.0.0)
cocoapods-stats (1.1.0)
cocoapods-trunk (1.4.1)
cocoapods-try (1.1.0)
colored2 (3.1.2)
concurrent-ruby (1.1.5)
crass (1.0.6)
csv (default: 3.0.9)
date (default: 2.0.0)
dbm (default: 1.0.0)
did_you_mean (1.3.0)
e2mmap (default: 0.1.0)
erubi (1.9.0)
escape (0.0.4)
etc (default: 1.0.1)
fcntl (default: 1.0.0)
fiddle (default: 1.0.0)
fileutils (default: 1.1.0)
forwardable (default: 1.2.0)
fourflusher (2.3.1)
fuzzy_match (2.0.4)
gh_inspector (1.1.3)
globalid (0.4.2)
httpclient (2.8.3)
i18n (0.9.5)
io-console (default: 0.4.7)
ipaddr (default: 1.2.2)
irb (default: 1.0.0)
json (default: 2.1.0)
libxml-ruby (3.1.0)
logger (default: 1.3.0)
loofah (2.6.0)
mail (2.7.1)
marcel (0.3.3)
matrix (default: 0.1.0)
method_source (1.0.0)
mimemagic (0.3.5)
mini_mime (1.0.2)
mini_portile2 (2.4.0)
minitest (5.11.3)
molinillo (0.6.6)
mutex_m (default: 0.1.0)
nanaimo (0.2.6)
nap (1.1.0)
net-telnet (0.2.0)
netrc (0.11.0)
nio4r (2.5.2)
nokogiri (1.10.1)
openssl (default: 2.1.2)
ostruct (default: 0.1.0)
power_assert (1.1.3)
prime (default: 0.1.0)
psych (default: 3.1.0)
rack (2.2.3)
rack-test (1.1.0)
rails (6.0.3.2)
rails-dom-testing (2.0.3)
rails-html-sanitizer (1.3.0)
railties (6.0.3.2)
rake (12.3.2)
rdoc (default: 6.1.0)
rexml (default: 3.1.9)
rss (default: 0.2.7)
ruby-macho (1.4.0)
scanf (default: 1.0.0)
sdbm (default: 1.0.0)
shell (default: 0.7)
sprockets (4.0.2)
sprockets-rails (3.2.1)
sqlite3 (1.3.13)
stringio (default: 0.0.2)
strscan (default: 1.0.0)
sync (default: 0.5.0)
test-unit (3.2.9)
thor (1.0.1)
thread_safe (0.3.6)
thwait (default: 0.1.0)
tracer (default: 0.1.0)
tzinfo (1.2.5)
webrick (default: 1.4.2)
websocket-driver (0.7.3)
websocket-extensions (0.1.5)
xcodeproj (1.13.0)
xmlrpc (0.3.0)
zeitwerk (2.4.0)
zlib (default: 1.0.0)


==> rails -v
Rails 6.0.3.2

~~~

### 41) Install Bundler

sudo gem install bundler

### 42) Install nokogiri

sudo gem install nokogiri

### 43) Create Gemfile for Jekyll

gem 'github-pages'
source 'https://rubygems.org'

### 44) Run bundle install : Run this command in the directory that contains the above Gemfil

bundle install

### 45) Install jekyll as described here :

https://www.taniarascia.com/make-a-static-website-with-jekyll/

jekyll new myjekyll


### 46) Brew install blade

https://github.com/jondot/blade

 $ brew tap jondot/tap
 $ brew install blade

### 47) IntelliJIdeaC

Install IntelliJIdeaC from 

https://www.jetbrains.com/idea/?fromMenu#chooseYourEdition

Import settings from intellij-idea-community-settings folder


### 48) Install Google Cloud SDK 
Install Cloud Tools version (156.0.0 at the time of authoring) from 

http://cloud.google.com/sdk/docs/nstall the latest Cloud Tools version (156.0.0)


### 49) Install postgres

==> brew install postgresql
Install postgres from 
http://postgresapp.com/

Configure your $PATH to use the included command line tools (optional):
sudo mkdir -p /etc/paths.d &&
echo /Applications/Postgres.app/Contents/Versions/latest/bin | sudo tee /etc/paths.d/postgresapp

### 50) Install pgAdmin
Install pgAdmin from 
https://www.pgadmin.org/download/


### 51) Install Heroku CLI 

Install Heroku CLI from steps
https://devcenter.heroku.com/articles/heroku-cli

brew tap heroku/brew && brew install heroku

### Workaround for M1 Apple Silicon mac

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

### 52) Install latest Java

Check Java version by using 
~~~
==> /usr/libexec/java_home

/Library/Java/JavaVirtualMachines/1.6.0.jdk/Contents/Hom
~~~

Install latest Java by downloading from
http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html

Check that latest Java was installed by using 

~~~
==> /usr/libexec/java_home
/Library/Java/JavaVirtualMachines/jdk1.8.0_231.jdk/Contents/Home

export JAVA_HOME in ~/.bashrc
export JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk1.8.0_231.jdk/Contents/Home
~~~

### 53) Install sdkman and gradle
https://sdkman.io

curl -s "https://get.sdkman.io" | bash

Install sdkman and grails as described here 
http://guides.grails.org/creating-your-first-grails-app/guide/index.html

$ curl -s "https://get.sdkman.io" | bash

$ sdk install grails

Check that latest grails was installed using 

==> grails -version
| Grails Version: 3.2.9
| Groovy Version: 2.4.10
| JVM Version: 1.8.0_131

### 54) Install pip 
Install pip as follows
sudo easy_install pip


### 55) Install awswebcli
Install EB CLI as follows

http://docs.aws.amazon.com/elasticbeanstalk/latest/dg/eb-cli3-install-osx.html

brew update

brew install awsebcli


### 56) Install mysql

Download and install mysql server from 

https://dev.mysql.com/downloads/mysql/

==> brew unlink mysql-connector-c
Unlinking /usr/local/Cellar/mysql-connector-c/6.1.10... 48 symlinks removed


==> brew install mysql

### 57) Install sublimetext3 snippets 

Install sublimetext3 snippets as described here :

https://github.com/arunabhdas/snippets

58) Set indentation on sublimetext3 to 4 spaces 

Set indentation to 4 spaces as described here :

https://stackoverflow.com/questions/22529265/sublime-text-3-convert-spaces-to-tabs


### 58) Add super+sift+f to key-bindings

Preferences -> Key Bindings
[
    { "keys": ["super+shift+f"], "command": "reindent"}
    
]

### 59) Check ruby env as follows

==> bundle env
- Environment

```
Bundler       1.16.1
  Platforms   ruby, x86_64-darwin-17
Ruby          2.5.0p0 (2017-12-25 revision 61468) [x86_64-darwin17]
  Full Path   /Users/das/.rubies/ruby-2.5.0/bin/ruby
  Config Dir  /Users/das/.rubies/ruby-2.5.0/etc
RubyGems      2.7.3
  Gem Home    /Users/das/.gem/ruby/2.5.0
  Gem Path    /Users/das/.gem/ruby/2.5.0:/Users/das/.rubies/ruby-2.5.0/lib/ruby/gems/2.5.0
  User Path   /Users/das/.gem/ruby/2.5.0
  Bin Dir     /Users/das/.gem/ruby/2.5.0/bin
Tools         
  Git         2.16.2
  RVM         
rvm 1.21.6 (stable) by Wayne E. Seguin <wayneeseguin@gmail.com>, Michal Papis <mpapis@gmail.com> [https://rvm.io/]


  rbenv       not installed
  chruby      0.3.9
```

- Bundler Build Metadata

```
Built At          2017-12-21
Git SHA           0034ef341
Released Version  true
```

- Bundler settings

```
```



### 60) Install rails as follows 

~~~
==> sudo gem install rails 
~~~
### 61) Install go

brew install go

## 62) Install Yarn

==> npm install -g yarn

### 63) Install Charles proxy

https://www.charlesproxy.com/documentation/proxying/ssl-proxying/

### 64) Install Postman
https://www.postman.com/downloads/

### 65) Install Paws

### 66) Install Stitch

### 67) Install Firefox

### 68) Install Mono, Fiddler
https://www.telerik.com/download/fiddler-wizard

### 69) Install pushpin 
http://pushpin.org/

### 70) Install Dart
brew tap dart-lang/dart
brew install dart --with-content-shell --with-dartium


### 71) Install VSCode
https://code.visualstudio.com/docs/?dv=osx


### 72) Install vim emulation for VSCode
https://github.com/VSCodeVim/Vim

### 73) Install rust

==> curl https://sh.rustup.rs -sSf | sh
info: downloading installer

Welcome to Rust!

This will download and install the official compiler for the Rust
programming language, and its package manager, Cargo.

It will add the cargo, rustc, rustup and other commands to
Cargo's bin directory, located at:

  /Users/das/.cargo/bin

This can be modified with the CARGO_HOME environment variable.

Rustup metadata and toolchains will be installed into the Rustup
home directory, located at:

  /Users/das/.rustup

This can be modified with the RUSTUP_HOME environment variable.

This path will then be added to your PATH environment variable by
modifying the profile files located at:

  /Users/das/.profile
/Users/das/.bash_profile

You can uninstall at any time with rustup self uninstall and
these changes will be reverted.

Current installation options:


   default host triple: x86_64-apple-darwin
     default toolchain: stable
               profile: default
  modify PATH variable: yes

1) Proceed with installation (default)
2) Customize installation
3) Cancel installation
>1

info: profile set to 'default'
info: updating existing rustup installation


Rust is installed now. Great!

To get started you need Cargo's bin directory ($HOME/.cargo/bin) in your PATH
environment variable. Next time you log in this will be done
automatically.

To configure your current shell run source $HOME/.cargo/env

==> rustc --version
rustc 1.39.0 (4560ea788 2019-11-04)

### 73) Git completion

~~~
==> brew install git bash-completion
~~~


### 74) Install Python Toolchain | Poetry

https://poetry.eustace.io/docs/

https://johnfraney.ca/posts/2019/05/28/create-publish-python-package-poetry/

https://dan.yeaw.me/posts/python-packaging-with-poetry-and-briefcase/

curl -sSL https://raw.githubusercontent.com/sdispater/poetry/master/get-poetry.py | python


### 75) Install Python Toolchain | Streamlit

https://streamlit.io/


### 76) Install Jhipster

npm install -g generator-jhipster


### 77) Install mvn

==> brew update

==> brew install maven


export M2_HOME=/usr/local/Cellar/maven/3.6.2/libexec
export M2=${M2_HOME}/bin
export PATH=${PATH}:${M2_HOME}/bin

### 78) Install docker

Install docker for mac
https://docs.docker.com/v17.12/docker-for-mac/install/


### 79) Install yarn

==> npm install -g yarn


### 80) Install pip 

sudo easy_install pip


### 81) Install hyper

Install hyper from here :

https://hyper.is/


### 82) Install nativescript

Install nativescript CLI as described here : 

npm install -g nativescript

### 83) Install flutter

https://flutter.dev/docs/get-started/install/macos


### 84) Install awscli
Install awscli from steps described here
https://docs.aws.amazon.com/cli/latest/userguide/install-macos.html#install-bundle-macos

~~~
curl "https://s3.amazonaws.com/aws-cli/awscli-bundle.zip" -o "awscli-bundle.zip"
unzip awscli-bundle.zip
sudo ./awscli-bundle/install -i /usr/local/aws -b /usr/local/bin/aws
~~~

## 85) Install anaconda using brew

~~~
brew install --cask anaconda
...
PREFIX=/usr/local/anaconda3
...

Add to .bashrc - 

# Anaconda path munging
export PATH=${PATH}:/usr/local/anaconda3/bin
~~~

Run 

~~~
jupyter notebook
~~~

### 86) Install Pytorch 

https://pytorch.org/get-started/locally/

### 87) Install Flutter

https://docs.flutter.dev/get-started/install/macos


### 87) Install Adobe

Install Adobe Creative Cloud

### 88) Install pnpm

```
npm install -g pnpm
```

