Setup a initiatory environment for web devlopment
============================================

This tutorial will teach you how to setup a environment for web devlopment with basic tools, follow the steps and you will get exactly these:

* Ubuntu
* Python + pip + virtualenv
* Vim + Markdown
* Git + Github
* zshell + oh-my-zsh

1. Ubuntu + Python
------------------

This is quite easy, download [ubuntu][1], burn it on a CD or USB and follow the instructions. Well, and you may use wubi also.

Python is contained in Ubuntu by default. In my case, Python 2.7.3 is distributed with Ubuntu 12.04 Desktop.

2. Git + Github
---------------
Install git by
	
	sudo apt-get install git

We use [Github][3] here to demostrate how to use git, basically of course.

First register on github, then click `New repository` to create a new repo on github. You'll see the instruction by github, follow that.

3. zshell + oh-my-zsh
---------------------

Zshell is a substitution for bash, people say it's better, but if you are satisfied with bash, skip this.

First we'll need to install zshell.

	sudo apt-get install zsh

Now you've got zshell and can enter it by the command `zsh`. Most people who install zshell would make it the default shell.

	chsh -s /bin/zsh

You may need to restart before this take effects.

Like many linux product, it has to be configured. There happened to be a popular config script call *oh-my-zsh*.

	git clone git://github.com/robbyrussell/oh-my-zsh.git ~/.oh-my-zsh
	cp ~/.oh-my-zsh/templates/zshrc.zsh-template ~/.zshrc

4. Vim + Markdown
-----------------
This tutorial is just written in Vim, pretty editor, i would say.

	sudo apt-get install vim

This gives you vim and config then. Add the following to `vimrc`(Mine's at `/etc/vim`).

	set tabstop=4
	set expandtab
	set shiftwidth=4
	set autoindent
	set smartindent

Google for some other settings and choose what you like.

**Something about Vim**  
I don't think it's a good idea to make Vim a giant IDE, though many people do and have their reasons. It's just a smart text editor, convieniant for small changes, or used in ssh. You don't need to put your project in Vim, IDEs do that, will you someday write a mass of code on your production server via ssh?
So what you need is just, like

* Fast cursor movements
* Skills and tricks of editing, like cut, copy, paste, insert.

Learn done.

For markdown support, checkout [this][2]

5. pip + virtualenv
-------------------
Pip is a tool for managing python packages, make install and remove them easier.
	
	sudo apt-get install python-pip

Virtualenv is another tool for managing python environments, help you shift between independent python environment.

	pip install virtualenv

[1]: http://www.ubuntu.com/ "Ubuntu"
[2]: https://github.com/plasticboy/vim-markdown "vim-markdown"
[3]: https://github.com/ "Github"
