---
permalink: "/cs110/programming_environment.html"
layout: cs110_page
title: Programming Environment Setup
exclude: true
---

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
[PyCharm](https://www.jetbrains.com/pycharm/download/#section=linux) (Community Edition).

> To test your environment, download and unzip the
[dummy project](https://www.cs.umb.edu/~siyer/teaching/cs110/dummy_project.zip) under `~/workspace`, launch PyCharm and open `~/workspace/dummy_project`, and run the following command on the PyCharm terminal:
```
$ python3 helloworld.py
```

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
$ echo "export PYTHONPATH=.:$HOME/lib/stdlib-python" >> $HOME/.zshenv
```

> Download and install
[PyCharm](https://www.jetbrains.com/pycharm/download/#section=mac) (Community Edition).

> To test your environment, download and unzip the
[dummy project](https://www.cs.umb.edu/~siyer/teaching/cs110/dummy_project.zip) under `~/workspace`, launch PyCharm and open `~/workspace/dummy_project`, and run the following command on the PyCharm terminal:
```
$ python3 helloworld.py
```

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
[PyCharm](https://www.jetbrains.com/pycharm/download/#section=windows) (Community Edition).

> To test your environment, download and unzip the
[dummy project](https://www.cs.umb.edu/~siyer/teaching/cs110/dummy_project.zip) under `~/workspace`, launch PyCharm and open `~/workspace/dummy_project`, and run the following command on the PyCharm terminal:
```
$ python.exe helloworld.py
```
