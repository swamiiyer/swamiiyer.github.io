---
permalink: "/cs451/programming_environment.html"
layout: cs451_page
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
> Install OpenJDK and ant.
```
$ sudo apt-get install openjdk-21-jdk ant
```
>
> Create `workspace` folder.
```
$ mkdir workspace
```

> Download and install [Visual Studio Code](https://code.visualstudio.com/sha/download?build=stable&os=linux-deb-x64) (aka VSCode). 
> 
> Launch VSCode, click on the Extensions icon on the left sidebar, search for the *Extension Pack for Java* extension and install it. 

> To test your environment, download and unzip the base [*j\-\-*](https://www.cs.umb.edu/~siyer/teaching/j--.zip) and [*iota*](https://www.cs.umb.edu/~siyer/teaching/iota.zip) compilers under `~/workspace`. 
>
> Launch VSCode, open the folder `~/workspace/j--`, and run the following commands in the VSCode terminal (can be launched by selecting *Terminal &rarr; New Terminal*): 
```
$ ant
```
>
```
$ chmod +x ./bin/j-- ./bin/javaccj-- ./bin/clemitter
```
>
```
$ ./bin/j-- tests/HelloWorld.java
```
>
```
$ java HelloWorld
```
>
> Launch VSCode, open the folder `~/workspace/iota`, and run the following commands in the VSCode terminal:
```
$ ant
```
>
```
$ chmod +x ./bin/iota
```
>
```
$ ./bin/iota tests/Factorial.iota
```
> 
```
$ python3 ./bin/marvin.py Factorial.marv
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
> Install brew.
```
$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
>
> Install OpenJDK and ant.
```
$ brew install openjdk@21 ant
```
> Set the environment variable `JAVA_HOME`.
```
$ echo "export JAVA_HOME=/opt/homebrew/opt/openjdk@21" >> $HOME/.zshenv
```
>
> Create `workspace` folder.
```
$ mkdir workspace
```

> Download [Visual Studio Code](https://code.visualstudio.com/sha/download?build=stable&os=darwin-universal) (aka VSCode), unzip the file, and move the extracted application into the *Applications* folder.
> 
> Launch VSCode, click on the Extensions icon on the left sidebar, search for the *Extension Pack for Java* extension and install it.

> To test your environment, download and unzip the base [*j\-\-*](https://www.cs.umb.edu/~siyer/teaching/j--.zip) and [*iota*](https://www.cs.umb.edu/~siyer/teaching/iota.zip) compilers under `~/workspace`.  
>
> Launch VSCode, open the folder `~/workspace/j--`, and run the following commands in the VSCode terminal (can be launched by selecting *Terminal &rarr; New Terminal*):  
 ```
$ ant
```
>
```
$ chmod +x ./bin/j-- ./bin/javaccj-- ./bin/clemitter
```
>
```
$ ./bin/j-- tests/HelloWorld.java
```
>
```
$ java HelloWorld
```
> 
> Launch VSCode, open the folder `~/workspace/iota`, and run the following commands in the VSCode terminal:
```
$ ant
```
>
```
$ chmod +x ./bin/iota
```
>
```
$ ./bin/iota tests/Factorial.iota
```
>
```
$ python3 ./bin/marvin.py Factorial.marv
```

<a name="win"/>
### Windows

> Launch a powershell terminal and run the following commands:
>
> Change to your home folder.
```
$ cd $HOME
```
>
> Create `workspace` folder
```
$ mkdir workspace
```
>

> Download and unzip [OpenJDK 21](https://download.java.net/java/GA/jdk21.0.2/f2283984656d49d69e91c558476027ac/13/GPL/openjdk-21.0.2_windows-x64_bin.zip) for Windows under some folder, say `C:\jdk21`. Run the following commands in a powershell terminal:
>
> Set the environment variable `JAVA_HOME`.
```
$ setx JAVA_HOME "C:\jdk21"
```
>
> Update the environment variable `PATH` to include the `C:\jdk21\bin`
folder.
```
$ setx PATH "$env:PATH;C:\jdk21\bin"
```

> Download and unzip
> [Ant](https://dlcdn.apache.org//ant/binaries/apache-ant-1.10.14-bin.zip)
> under some folder, say `C:\ant`.  Run the following command in a powershell terminal: 
>
> Update the environment variable `PATH` to include the `C:\ant\bin`
> folder.
```
$ setx PATH "$env:PATH;C:\ant\bin"
```

> Download and install [Visual Studio Code](https://code.visualstudio.com/sha/download?build=stable&os=win32-x64-user) (aka VSCode).
> 
> Launch VSCode, click on the Extensions icon on the left sidebar, search for the *Extension Pack for Java* extension and install it.

> Install [Python 3](https://www.python.org/downloads/),  making sure you have checked the box that says *Add Python 3.x to PATH*.

> To test your environment, download and unzip the base 
[*j\-\-*](https://www.cs.umb.edu/~siyer/teaching/j--.zip) and [*iota*](https://www.cs.umb.edu/~siyer/teaching/iota.zip) compilers under `~/workspace`.
>
> Launch VSCode, open the folder `~/workspace/j--`, and run the following commands in the VSCode terminal (can be launched by selecting *Terminal &rarr; New Terminal*):
```
$ ant
```
>
```
$ ./bin/j-- tests/HelloWorld.java
```
>
```
$ java HelloWorld
```
>
> Launch VSCode, open the folder `~/workspace/iota`, and run the following commands in the VSCode terminal:
```
$ ant
```
>
```
$ ./bin/iota tests/Factorial.iota
```
>
```
$ python.exe ./bin/marvin.py Factorial.marv
```
