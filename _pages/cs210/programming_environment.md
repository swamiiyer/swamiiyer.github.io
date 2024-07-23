---
permalink: "/cs210/programming_environment.html"
layout: cs210_page
title: Programming Environment Setup
exclude: true
---

### Select Your Operating System

- [**Ubuntu Linux**](#linux)

- [**Mac OS X**](#mac) 

- [**Windows**](#win) 

<a name="linux"/>
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
$ sudo apt-get install openjdk-21-jdk
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
> Set the environment variable `CLASSPATH`.
```
$ echo "export CLASSPATH=.:./out:$HOME/lib/stdlib.jar:$HOME/lib/dsa.jar" >> $HOME/.bashrc
```

> Download and install
[IntelliJ](https://www.jetbrains.com/idea/download/#section=linux) (Community Edition).

> To test your environment, download and unzip the [`dsaj.zip`](https://www.cs.umb.edu/~siyer/teaching/dsaj.zip) under `~/workspace`, launch IntelliJ, open the project `~/workspace/dsaj/programs`, and run the following commands in the IntelliJ terminal:
```
$ javac -d out src/HelloWorld.java
```
>
```
$ java HelloWorld
```

<a name="mac"/>
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
$ brew install openjdk@21 wget
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
> Set the environment variable `CLASSPATH`.
```
$ echo "export CLASSPATH=.:./out:$HOME/lib/stdlib.jar:$HOME/lib/dsa.jar" >> $HOME/.zshenv
```

> Download and install
[IntelliJ](https://www.jetbrains.com/idea/download/#section=mac) (Community Edition).

> To test your environment, download and unzip the [`dsaj.zip`](https://www.cs.umb.edu/~siyer/teaching/dsaj.zip) under `~/workspace`, launch IntelliJ, open the project `~/workspace/dsaj/programs`, and run the following commands in the IntelliJ terminal:
```
$ javac -d out src/HelloWorld.java
```
>
```
$ java HelloWorld
```

<a name="win"/>
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
> Set the environment variable `CLASSPATH`.
```
$ setx CLASSPATH ".;.\out;$HOME\lib\stdlib.jar;$HOME\lib\dsa.jar"
```

> Download and unzip [OpenJDK 21](https://download.java.net/java/GA/jdk21.0.2/f2283984656d49d69e91c558476027ac/13/GPL/openjdk-21.0.2_windows-x64_bin.zip) for Windows under some folder, say `C:\jdk21`. Run the following command in a powershell terminal:
>
> Update the environment variable `PATH` to include the `C:\jdk21\bin`
folder.
```
$ setx PATH "$env:PATH;C:\jdk21\bin"
```

> Download and install
> [IntelliJ](https://www.jetbrains.com/idea/download/#section=windows)
> (Community Edition). Launch IntelliJ, go to *Configure* &rarr; *Settings* &rarr; *Tools* &rarr; *Terminal*, and set *Shell path* to `powershell`.

> To test your environment, download and unzip the [`dsaj.zip`](https://www.cs.umb.edu/~siyer/teaching/dsaj.zip) under `~/workspace`, launch IntelliJ, open the project `~/workspace/dsaj/programs`, and run the following commands in the IntelliJ terminal:
```
$ javac -d out src/HelloWorld.java
```
>
```
$ java HelloWorld
```
