# **notes**
*Notes on learning the Go programming language*

## **Welcome!**
The purpose of these notes is to share with others my learning process as a complete beginner with no background in programming.
The notes have two tracks: one focusing on the Go language itself and another on the tools associated with Go. 
I suggest you first start in [Go playground](https://play.golang.org/) to learn Go basics before moving to work in a terminal.
We will start with a very simple program and gradually build upon it as we learn new concepts. The goal is to eventually have a complex program whose components you understand fully since you have built it from the ground up. To maximize learning, I advise you to try running programs on Go playground as you follow the notes.

To learn more about go, visit [Go website](https://golang.org/). 

## **Go from the start**
Go is a language made up of many packages. There are about [40 packages total](https://golang.org/pkg/) in the standard library. You can either import a package from the standard library or from a third party. Whenever you import a package, all components of that package (functions, types, methods) are imported as well. Let's start with a simple program in [Go playground](https://play.golang.org/):
```
package main

import "fmt"

func main() {
  fmt.Println("Hi there, fellow Gophers!")
}

```
Let us look at each element above. We start in main package by typing `package main` and importing a package called `fmt` which allows you to print an output of your program onto a terminal. The names of all imported packages are in double quotes. 

Main package contains one and only one main function. To define a function, you type `func` followed by the name of that function, in this case `main()`. A name of a function is followed by parentheses inside which you place arguments or inputs for that function. Main function takes no arguments. An output of a function goes right after the closing parenthesis. Main function returns no outputs. The body of a function is enclosed in curly brackets. 

Main unction can contain other functions which in turn have their own arguments inside parenttheses (?). You first type the name of the imported package followed by a dot and then the name of the function in that package starting in caps as in `fmt.Println`. There are several `Print` functions in `fmt`. Here, we used `Println` which allows you to print a line without needing to specify the end of the line (?). If you want to print text as it is you need to enclose it in double quotes. In Go, anything in double quotes is called a string. 

## **Tools for Go** ##
Now, I would like to introduce various tools that are needed for programming and share a few valuable tips.

## **Github**
It is a good idea to create a repository on [github](https://github.com) where you can store your code and share your work with others.
TODO: add on git pull, push, etc...

## **Terminals**
You need a terminal to do any programming work. A terminal is an interface where you can type, edit and execute your programs.
It is a good idea to use tmux, a terminal multiplexer, that allows you to have multiple windows open and to swtich easily between these windows.
If you are using a macbook, use a finder to search for a terminal. Every macbook should have a terminal.
Once you open a terminal, type *tmux attach* to open tmux.
Usually, source code is entered and edited on emacs...


