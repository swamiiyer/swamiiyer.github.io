---
permalink: "/cs110/programming_environment.html"
layout: cs110_page
title: Programming Environment Setup
exclude: true
---

### Select Your Operating System

- [**Ubuntu Linux**](#linux)

- [**Mac OS X**](#mac) 

- [**Windows**](#win) 

<a name="linux"/>
### Ubuntu Linux

> Launch a terminal and run the following commands:
>
> Change to your home folder.
```
$ cd $HOME
```
>
> Install `python3-pip` and `python3-tk`.
```
$ sudo apt-get install python3-pip python3-tk
```
>
> Install `numpy` and `pygame`.
```
$ pip3 install numpy pygame
```
>
> Create `lib` and `workspace` folders.
```
$ mkdir lib workspace
```
>
> Download `stdlib-python.zip`.
```
$ wget https://www.cs.umb.edu/~siyer/teaching/stdlib-python.zip
```
>
> Unzip `stdlib-python.zip` under ~/lib.
```
$ unzip stdlib-python.zip -d lib
```
>
> Remove `stdlib-python.zip`.
```
$ rm stdlib-python.zip
```
>
> Set the environment variable `PYTHONPATH`.
```
$ echo "export PYTHONPATH=.:$HOME/lib/stdlib-python" >> $HOME/.bashrc
```

> Download and install
[Visual Studio Code](https://code.visualstudio.com/sha/download?build=stable&os=linux-deb-x64) (aka
VSCode).

> Launch VSCode, click on the Extensions icon on the left sidebar, search for
> the Python extension, and install it.

> To test your environment, download and unzip
[`ipp.zip`](https://www.cs.umb.edu/~siyer/teaching/ipp.zip) under
`~/workspace`, launch VSCode, open the folder `~/workspace/ipp`, and
run the following commands in the VSCode terminal (can be launched by selecting *Terminal &rarr; New Terminal*):
```
$ python3 helloworld.py 
```
```
$ python3 bouncingball.py 
```
```
$ python3 playthattune.py < data/looney.txt 
```

<a name="mac"/>
### Mac OS X

> Launch a terminal and run the following commands: 
>
> Change to your home folder.
```
$ cd $HOME
```
>
> Install `brew`.
```
$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
>
> Install `python-tk` and `wget`.
```
$ brew install python-tk wget
```
>
> Install `numpy` and `pygame`.
```
$ pip3 install numpy pygame --break-system-packages
```
>
> Create `lib` and `workspace` folders.
```
$ mkdir lib workspace
```
>
> Download `stdlib-python.zip`.
```
$ wget https://www.cs.umb.edu/~siyer/teaching/stdlib-python.zip
```
>
> Unzip `stdlib-python.zip` under ~/lib.
```
$ unzip stdlib-python.zip -d lib
```
>
> Remove `stdlib-python.zip`.
```
$ rm stdlib-python.zip
```
>
> Set the environment variable `PYTHONPATH`.
```
$ echo "export PYTHONPATH=.:$HOME/lib/stdlib-python" >> $HOME/.zshenv
```

> Download [Visual Studio Code](https://code.visualstudio.com/sha/download?build=stable&os=darwin-universal) (aka
VSCode), unzip the file, and move the extracted application into the
*Applications* folder.

> Launch VSCode, click on the Extensions icon on the left sidebar, search for
> the Python extension, and install it.

> To test your environment, download and unzip
[`ipp.zip`](https://www.cs.umb.edu/~siyer/teaching/ipp.zip) under
`~/workspace`, launch VSCode, open the folder `~/workspace/ipp`, and
run the following commands in the VSCode terminal (can be launched by
selecting *Terminal &rarr; New Terminal*):

```
$ python3 helloworld.py 
```
```
$ python3 bouncingball.py 
```
```
$ python3 playthattune.py < data/looney.txt 
```

<a name="win"/>
### Windows

> Install [Python 3](https://www.python.org/downloads/),  making sure you have checked the box that says *Add
Python 3.x to PATH*.

> Launch a powershell terminal and run the following commands:
>
> Change to your home folder.
```
$ cd $HOME
```
>
> Install `numpy` and `pygame`.
```
$ pip3 install numpy pygame
```
>
> Create `lib` and `workspace` folders.
```
$ mkdir lib,workspace
```
>
> Download `stdlib-python.zip`.
```
$ wget -O stdlib-python.zip https://www.cs.umb.edu/~siyer/teaching/stdlib-python.zip
```
>
> Unzip `stdlib-python.zip` under `~/lib`.
```
$ Expand-Archive -LiteralPath stdlib-python.zip -DestinationPath lib
```
>
> Remove `stdlib-python.zip`.
```
$ rm stdlib-python.zip
```
>
> Set the environment variable `PYTHONPATH`.
```
$ setx PYTHONPATH ".;$HOME\lib\stdlib-python"
```

> Download and install
[Visual Studio Code](https://code.visualstudio.com/sha/download?build=stable&os=win32-x64-user) (aka
VSCode).

> Launch VSCode, click on the Extensions icon on the left sidebar, search for
> the Python extension, and install it.

> To test your environment, download and unzip
[`ipp.zip`](https://www.cs.umb.edu/~siyer/teaching/ipp.zip) under
`~/workspace`, launch VSCode, open the folder `~/workspace/ipp`, and
run the following commands in the VSCode terminal (can be launched by selecting *Terminal &rarr; New Terminal*):

```
$ python.exe helloworld.py 
```
```
$ python.exe bouncingball.py 
```
```
$ Get-Content data/looney.txt | python.exe playthattune.py
```
