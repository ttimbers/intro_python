# Setting Up

## Table of Contents
- [Getting and Installing Python](#getting-and-installing-python)
- [Installing Rodeo](#installing-rodeo)
- [Useful Terminal Commands](#three-useful-terminal-commands)
- [Documentation](#documentation)
- [Troubleshooting](#troubleshooting)


## Getting and Installing Python

We will be using Python for a large part of the program, including many popular 3rd party Python libraries for scientific computing. [__Anaconda__](https://docs.continuum.io/) is an easy-to-install bundle of Python and most of these libraries. We __strongly recommend__ that you use Anaconda for this program. If you insist on using your own Python setup instead of Anaconda, we will not be able to provide the same level of support with installation.

For this program we are using __Python 3__ , not __Python 2__, so please chose the Anaconda versions that include Python 3.5

#### Mac/Linux Users

1. Head to https://www.continuum.io/downloads and download the Anaconda version for Mac OS with Python 3.5.
2. Follow the instructions on that page to run the installer
3. Test out the Jupyter notebook: open a Terminal window, and type ```jupyter notebook```. Or use the Anaconda Launcher which might have been deposited on your desktop. A new browser window should pop up.
4.	Click New Notebook to create a new notebook file. __Trick__: give this notebook a unique name, like *my-little-rose* and save it. Use Spotlight (upper right corner of the mac desktop, looks like a maginifier) to search for this name. In this way, you will know which folder your notebook opens in by default.  

If you already have installed Anaconda at some point in the past, you can easily update to the latest Anaconda version by updating conda, then Anaconda in terminal as follows:
```
	conda update conda
    conda update anaconda    
```


#### Windows Users

1. Head to https://www.continuum.io/downloads and download the Anaconda version with Python 3.5.
2. Follow the instructions on that page to run the installer
3. Test it out: start the Anaconda launcher, which you can find in ```C:\Anaconda``` or, in the Start menu. Start the Jupyter notebook. A new browser window should open.
4.	Click New Notebook, which should open a new page. Trick: give this notebook a unique name, like *my-little-rose* and save it. Use Explorer (usually start menu on windows desktops) to search for this name. In this way, you will know which folder your notebook opens in by default.

### __Running Jupyter Notebook__
The Jupyter notebook is an application to build interactive computational notebooks.

When you open Jupyter, you should see a page similar to this:

![first_time](https://www.dropbox.com/s/1hasj11i1hj340x/settingup.JPG?dl=1)

To create a new notebook go to *New -> Python 3*.

Notebooks are composed of many "cells", which can contain text  or code (like the one below). Create a cell like the one below, and evaluate the python code by clicking the "play" button above, or by hitting ```Ctrl + enter```

![](https://www.dropbox.com/s/nbkbqq2nliykfr6/settingup1.JPG?dl=1)

Now go to *Insert -> Insert New Cell Below* and run the following code in this new cell:
```
import numpy
import scipy
import matplotlib
```

![](https://www.dropbox.com/s/bf6gr7d8bx3m8xj/settingup2.JPG?dl=1)


numpy, scipy and matplotlib are some of the important libraries that come with Anaconda that we will be using. Now instead of using ```Ctrl + enter ``` to run your code, try ```shift + enter```. Using this, Jupyter will run your code *and* create a new cell automatically. If this code runs successfully, you should have a successful installation of Anaconda!

## Installing Rodeo
Rodeo is an easy-to-use Python IDE (Integrated Development Environment) based on Jupyter. Rodeo will allow us to write our Python code and run it, and comes with other data-science specific features.


#### Mac Users
1. Download Rodeo [here](https://www.yhat.com/products/rodeo/downloads). If your download doesn't start automatically, download the Mac version.
2. Double-click the Rodeo-mac.dmg file you downloaded.
3. Drag the Rodeo app icon to your Applications folder.
4. Double-click the Rodeo icon in your Applications folder.

#### Linux Users
1. Download Rodeo [here](https://www.yhat.com/products/rodeo/downloads). If your download doesn't start automatically, select the appropriate(32-bit or 64-bit) version for Linux.
2. Unzip Rodeo into your applications directory (i.e. ```~/bin/```).
3. Add the ```Rodeo``` command to your path, then execute it to start Rodeo!

You can also execute the following commands in terminal instead:
```
wget -O tmp.zip https://www.yhat.com/products/rodeo/downloads/linux_64
sudo unzip tmp.zip -d /usr/local/bin/ && rm tmp.zip
sudo ln -s /usr/local/bin/Rodeo-linux-x64/Rodeo /usr/local/bin
```
Change 64 to 32 in the first and last command if you have a 32-bit system.

#### Windows Users
1. Download Rodeo [here](https://www.yhat.com/products/rodeo/downloads). If your download doesn't start automatically, select and download the appropriate (32-bit or 64-bit) Windows version.
2. Open the installer and install with defaults.
3. Launch Rodeo from your start-menu (or where you installed it).

## Installing a Text Editor
We need a text editor to be able to write complete applications. We will be using the open-source editor Atom.

## Three Useful Terminal Commands


You can use the terminal to navigate through your computer’s file system and run various applications. Windows users should use Git Bash(search for it in Start Menu), while Mac/Linux Users should open their terminals. Here are some useful commands that you should be familiar with(try them out!):

- ```pwd```  - shows the path of your current directory (i.e. tells you where you are)
on Windows, the terminal prompt contains the path of your current directory
- ```ls``` shows what is in the current directory
- ```cd <directory or path> ``` - change directory to the specified directory (**NOTE**: the use of the greater than and less than signs are meant to indicate that you need to type in whatever directory or path you want to go to. You should not literally type in these symbols into the terminal)
	-	```cd ..``` goes up one level, to the parent folder
	- *extra tip*: TAB does autocomplete for file names (start typing the name of a file/folder and press TAB before you finish typing)
 	- You can use the symbol ```~```as shorthand for your home directory. So for example ```cd ~/Desktop``` will probably get you to your desktop if you're on Mac/Linux. **Note**: This references an *absolute* path rather than a *relative* path -- it points directly to your home directory regardless of what directory you are currently in, rather than some place relative to the current directory you are in. The rest of the time when you use cd to navigate around you are usually specifying relative paths (path relative to where you are right now).

1.	Chose a folder where you want to save your work for this assignment.
2.	Open Atom, and write the following code:
```print test successful!``` and then go to *File -> Save As* and save the file with the extensiion ```.py``` in the directory you chose. For example, I saved the file as *test.py*.  

3.	Now, in terminal, navigate to that folder using the commands you learned above.
4.	Once you are there, type:
```python <program name>.py ```. In this case, we type ```python test.py```. You should now see ```test successful!``` in your terminal.

You can do a lot more with a terminal. See software carpentry's [resources](http://swcarpentry.github.io/shell-novice/) on this.


## Documentation

The following resources will be very helpful in explaining how to work with the required languages and environments.

[Python 3.5](https://docs.python.org/3/)


[Jupyter Notebook](http://jupyter.readthedocs.io/en/latest/)


[Useful UNIX commands](http://mally.stanford.edu/~sr/computing/basic-unix.html)



## Troubleshooting

A lot of these questions are answered on [StackOverflow](http://stackoverflow.com/). We encourage you to use StackOverflow throughout the program.


## Acknowledgements
* [UBC Stat545](stat545.com) Taught by: Jennifer Bryan
* [Harvard CS109](http://cs109.github.io/2015/)
