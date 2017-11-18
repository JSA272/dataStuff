# Quick instructions for setting up homebrew, r, and mysql
This might sound crazy, but you can do it! You will feel super cool once you've done this

Mac OS has an application called Terminal preinstalled. Open it up and you'll see an old-school text box. The terminal is like the secret back door to your computer that gives you immense power and control if you're willing to learn how to use it. For our purposes here, the Terminal will allow us to easily install the programs we need, and allow the programs to know how to find each other once they're installed. In the future, you'll start using the Terminal more and more to do your work, so now's a good time to start.

1. Install XCode Command Line Tools

    * XCode is a program made by Apple which allows people to create iPhone apps and stuff. You could install the whole thing, but since it's pretty large, we're only going to install the part we need to get Homebrew running, the Command Line Tools.
    * Run `xcode-select --install` from the terminal.
    * A message box will appear asking if you want to install the Command Line Tools answer yes, but don't install the entire XCode program. If you do, it's not the end of the world, but I'm trying to save some disk space.
  
1. Install Homebrew

    * Now we can install Homebrew, a package manager for terminal software. It will allow us to easily install r and mysql from the command line, and automatically download any additional software you might need.
    * Copy this to the terminal: `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`. Homebrew will download automatically.
    
1. Install R and Mysql

    * The hard part is over! Now we can quickly install R and mysql using Homebrew.
    * Run `brew install r` and `brew install mysql`. After each command, you will see messages describing the download process.
    * You now have these programs on your computer. Use the command `brew list` to have Homebrew list everything it has downloaded. R and Mysql should be included.
    
1. Install RStudio and Mysql Workbench

    * In the previous step, we installed R and Mysql, but these were just the "backend" versions of the programs, which are cumbersome to use on their own. When we're actually doing work, we want a "frontend" program to make them easier to use. For R and Mysql, I use Rstudio and Mysql Workbench, respectively.
    * Homebrew alone can only install terminal software, but there is a useful extention called Hombrew Cask that can easily install other software
    * To set up the homebrew cask, type `brew tap caskroom/cask` in the terminal.
    * Run `brew cask install rstudio` and `brew cask install mysqlworkbench`. Everything is now installed
    * You can type `brew cask list` to see everything installed from the Homebrew Cask. Rstudio and Mysql Workbench should be there.
    
Let me know if you get any weird errors during this process. If all goes well, I can show you how everything goes together next week.
