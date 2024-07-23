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

> Download and install
[IntelliJ](https://www.jetbrains.com/idea/download/#section=linux) (Community Edition).

> To test your environment, download and unzip the base 
[*j\-\-* compiler](https://www.cs.umb.edu/~siyer/teaching/j--.zip) and [*iota*](https://www.cs.umb.edu/~siyer/teaching/iota.zip) compilers under `~/workspace`.
>
> Launch IntelliJ, open `~/workspace/j--`, and run the following commands in the IntelliJ terminal:
```
$ ant
```
>
```
$ chmod +x ./bin/j--
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
> Launch IntelliJ, open `~/workspace/iota`, and run the following commands in the IntelliJ terminal:
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
> Open `~/workspace/iota/Factorial.hmmm` in [HMMM Simulator](https://shickey.github.io/HMMM.js/#/), assemble the instructions, and simulate/run the assembled binary code. Alternatively, you can run `Factorial.hmmm` in the terminal as follows:
```
$ python3 ./bin/hmmm Factorial.hmmm
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
>
> Create `workspace` folder.
```
$ mkdir workspace
```

> Download and install
[IntelliJ](https://www.jetbrains.com/idea/download/#section=mac) (Community Edition).

> To test your environment, download and unzip the base 
[*j\-\-* compiler](https://www.cs.umb.edu/~siyer/teaching/j--.zip) and [*iota*](https://www.cs.umb.edu/~siyer/teaching/iota.zip) compilers under `~/workspace`.
>
> Launch IntelliJ, open `~/workspace/j--`, and run the following commands in the IntelliJ terminal:
```
$ ant
```
>
```
$ chmod +x ./bin/j--
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
> Launch IntelliJ, open `~/workspace/iota`, and run the following commands in the IntelliJ terminal:
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
> Open `~/workspace/iota/Factorial.hmmm` in [HMMM Simulator](https://shickey.github.io/HMMM.js/#/), assemble the instructions, and simulate/run the assembled binary code. Alternatively, you can run `Factorial.hmmm` in the terminal as follows:
```
$ python3 ./bin/hmmm Factorial.hmmm
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
$ setx JAVA_HOME "C:\jdk21\bin"
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

> Download and install [IntelliJ](https://www.jetbrains.com/idea/download/#section=windows) (Community Edition). Launch IntelliJ, go to *Configure* &rarr; *Settings* &rarr; *Tools* &rarr; *Terminal*, and set *Shell path* to `powershell`.

> To test your environment, download and unzip the base 
[*j\-\-* compiler](https://www.cs.umb.edu/~siyer/teaching/j--.zip) and [*iota*](https://www.cs.umb.edu/~siyer/teaching/iota.zip) compilers under `~/workspace`.
>
> Launch IntelliJ, open `~/workspace/j--`, and run the following commands in the IntelliJ terminal:
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
> Launch IntelliJ, open `~/workspace/iota`, and run the following commands in the IntelliJ terminal:
```
$ ant
```
>
```
$ ./bin/iota tests/Factorial.iota
```
> Open `~/workspace/iota/Factorial.hmmm` in [HMMM Simulator](https://shickey.github.io/HMMM.js/#/), assemble the instructions, and simulate/run the assembled binary code. Alternatively, you can `Factorial.hmmm` in the terminal as follows:
```
$ python.exe ./bin/hmmm Factorial.hmmm
```
