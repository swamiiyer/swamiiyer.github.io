---
permalink: "/cs210/programming_environment.html"
layout: cs210_page
title: Programming Environment Setup
exclude: true
---

## Ubuntu Linux

> Launch a terminal and run the following commands:
>
> Change to your home folder.
```
$ cd $HOME
```
>
> Install `OpenJDK`.
```
$ sudo apt-get install openjdk-17-jdk
```
>
> Create `lib` and `workspace` folders.
```
$ mkdir lib workspace
```
>
> Download `stdlib.jar` under `~/lib`.
```
$ wget https://www.cs.umb.edu/~siyer/teaching/stdlib.jar -P lib
```
>
> Download `dsa.jar` under `~/lib`.
```
$ wget https://www.cs.umb.edu/~siyer/teaching/dsa.jar -P lib
```
>
> Set the environment variable `PROJECT_HOME`.
```
$ echo "export PROJECT_HOME=$HOME/workspace" >> $HOME/.bashrc
```
>
> Set the environment variable `CLASSPATH`.
```
$ echo "export CLASSPATH=.:./out:$HOME/lib/stdlib.jar:$HOME/lib/dsa.jar" >> $HOME/.bashrc
```

> Download and install
[IntelliJ](https://www.jetbrains.com/idea/download/#section=linux) (Community Edition).

> To test your environment, download and unzip the
[dummy project](https://www.cs.umb.edu/~siyer/teaching/cs210/dummy_project.zip) under `~/workspace`, launch IntelliJ and open `~/workspace/dummy_project`, and run the following commands on the IntelliJ terminal:
```
$ javac -d out src/HelloWorld.java
```
>
```
$ java HelloWorld
```

## Mac OS X

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
> Install `OpenJDK` and `wget`.
```
$ brew install openjdk@17 wget
```
>
> Create `lib` and `workspace` folders.
```
$ mkdir lib workspace
```
>
> Download `stdlib.jar` under `~/lib`.
```
$ wget https://www.cs.umb.edu/~siyer/teaching/stdlib.jar -P lib
```
>
> Download `dsa.jar` under `~/lib`.
```
$ wget https://www.cs.umb.edu/~siyer/teaching/dsa.jar -P lib
```
>
> Set the environment variable `PROJECT_HOME`.
```
$ echo "export PROJECT_HOME=$HOME/workspace" >> $HOME/.zshenv
```
>
> Set the environment variable `CLASSPATH`.
```
$ echo "export CLASSPATH=.:./out:$HOME/lib/stdlib.jar:$HOME/lib/dsa.jar" >> $HOME/.zshenv
```

> Download and install
[IntelliJ](https://www.jetbrains.com/idea/download/#section=mac) (Community Edition).

> To test your environment, download and unzip the
[dummy project](https://www.cs.umb.edu/~siyer/teaching/cs210/dummy_project.zip) under `~/workspace`, launch IntelliJ and open `~/workspace/dummy_project`, and run the following commands on the IntelliJ terminal:
```
$ javac -d out src/HelloWorld.java
```
>
```
$ java HelloWorld
```

## Windows

> Launch a powershell terminal and run the following commands:
>
> Change to your home folder.
```
$ cd $HOME
```
>
> Create `lib` and `workspace` folders.
```
$ mkdir lib,workspace
```
>
> Download `stdlib.jar` under `~/lib`.
```
$ wget -O lib\stdlib.jar https://www.cs.umb.edu/~siyer/teaching/stdlib.jar
```
>
> Download `dsa.jar` under `~/lib`.
```
$ wget -O lib\dsa.jar https://www.cs.umb.edu/~siyer/teaching/dsa.jar
```
>
> Set the environment variable `PROJECT_HOME`.
```
$ setx PROJECT_HOME "$HOME\workspace"
```
>
> Set the environment variable `CLASSPATH`.
```
$ setx CLASSPATH ".;.\out;$HOME\lib\stdlib.jar;$HOME\lib\dsa.jar"
```

> Download and unzip [OpenJDK
> 17](https://download.java.net/openjdk/jdk17/ri/openjdk-17+35_windows-x64_bin.zip)
> for Windows under some folder, say `C:\jdk17`. Run the following command in a powershell terminal:
>
> Update the environment variable `PATH` to include the `C:\jdk17\bin`
folder.
```
$ setx PATH "$env:PATH;C:\jdk17\bin"
```


> Download and install
> [IntelliJ](https://www.jetbrains.com/idea/download/#section=windows)
> (Community Edition). Launch IntelliJ, go to *Configure* &rarr; *Settings* &rarr; *Tools* &rarr; *Terminal*, and set *Shell path* to `powershell`.

> To test your environment, download and unzip the
[dummy project](https://www.cs.umb.edu/~siyer/teaching/cs210/dummy_project.zip) under `~/workspace`, launch IntelliJ and open `~/workspace/dummy_project`, and run the following commands on the IntelliJ terminal:
```
$ javac -d out src/HelloWorld.java
```
>
```
$ java HelloWorld
```
