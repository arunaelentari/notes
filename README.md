# **notes**
*Notes on learning the Go programming language*

## **Welcome!**
The purpose of these notes is to share with others my learning process as a complete beginner with no background in programming.
The notes have two tracks: one focusing on the Go language itself and another on the tools associated with Go. 
I suggest you first start in [Go playground](https://play.golang.org/) to learn Go basics before moving to work in a terminal.
We will start with a very simple program and build upon it as we learn new concepts. The goal is eventually to have a complex program whose components you can fully understand since you built it from the ground up.
To learn more about go, visit [Go website](https://golang.org/). 

## **Go from start**
Go is a language made up of many packages. There are about 40 packages total. A typical Go package contains various functions, methods, types and other things that you can import into your own program. Let's start with a simple program in [Go playground](https://play.golang.org/):
```
package main

import "fmt"

func main() {
  fmt.Println("Hello, world!")
}

```
Let us look at each element above. 
You always start your program by typing `package main` and importing a package called `fmt` which allows you to print an output of your program on a terminal. The names of all imported packages are in double quotes.

Every main package contains one and only one main function.


Before we start with Go, I would like to introduce various tools that are needed for programming and share a few valuable tips.

## **Github**
It is a good idea to create a repository on [github](https://github.com) where you can store your code and share your work with others.
TODO: add on git pull, push, etc...

## **Terminals**
You need a terminal to do any programming work. A terminal is an interface where you can type, edit and execute your programs.
It is a good idea to use tmux, a terminal multiplexer, that allows you to have multiple windows open and to swtich easily between these windows.
If you are using a macbook, use a finder to search for a terminal. Every macbook should have a terminal.
Once you open a terminal, type *tmux attach* to open tmux.
Usually, source code is entered and edited on emacs...


