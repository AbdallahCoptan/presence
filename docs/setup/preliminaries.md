
This projects relies on several components you need to have installed on your system.

* [Git](https://git-scm.com/)

The below instructions will help you to install these components, depending on your running platform.

_Note_: in the following instructions, terminal commands are prefixed by a virtual prompt `$>`which obviously **does not** belong to the command.

## Pre-requisites

* Install the following software, depending on your running platform:

| Platform | Software                                              | Description                           | Usage                   |
|----------|-------------------------------------------------------|---------------------------------------|-------------------------|
| Mac OS   | [Homebrew](http://brew.sh/)                           | The missing package manager for macOS | `brew install ...`      |
| Mac OS   | [Brew Cask Plugin](https://caskroom.github.io)        | Mac OS Apps install made easy         | `brew cask install ...` |
| Mac OS   | [iTerm2](https://www.iterm2.com/)                     | _(optional)_ enhanced Terminal        |                         |
| Windows  | [Git for Windows](https://git-for-windows.github.io/) | I'm sure you guessed                  |                         |
| Windows  | [SourceTree](https://www.sourcetreeapp.com/)          | _(optional)_ enhanced git GUI         |                         |
| Windows  | [Virtual Box](https://www.virtualbox.org/)            | Free hypervisor provider for Vagrant  |                         |
| Windows  | [Vagrant](https://www.vagrantup.com/downloads.html)   | Reproducible environments made easy.  |                         |


* Follow the below custom instructions depending on your running platform

### Mac OS X

Now that you have [Homebrew](http://brew.sh/) installed:

~~~bash
$> brew install git-core git-flow    # (newer) Git stuff
~~~

### Linux (Debian / Ubuntu)

~~~bash
$> sudo apt-get update
$> sudo apt-get install git build-essential
~~~

Adapt the package names (and package manager) in case you are using another Linux distribution.


### Windows

Follow the instructions provided on this [tutorial](http://rr-tutorials.readthedocs.io/en/latest/setup/#windows).
In particular, it may be a good idea to rely on [Vagrant](https://www.vagrantup.com/) to run a Linux box.


## Post-Installations checks

(Eventually) Make yourself known to Git

~~~bash
$> git config –-global user.name  "Firstname LastName"              # Adapt accordingly
$> git config –-global user.email "Firstname.LastName@domain.org"   # Adapt with your mail
~~~

Clone the [project repository](Gitlab @ Uni.luhttps://gitlab.uni.lu/aibrahim/presence from a Terminal (Powershell as `administrator` under windows):

~~~bash
$> mkdir -p ~/git/gitlab.uni.lu/aibrahim
$> cd ~/git/gitlab.uni.lu/aibrahim
$> git clone ssh://git@gitlab.uni.lu:8022/aibrahim/presence.git
$> rake setup    # Under Mac OS / Linux
~~~
