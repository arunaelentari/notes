#**notes**
*Notes on learning go and other languages*

##**Welcome!**
I thought it would be good to take notes as I am learning Go and other languages.
I try to structure my notes so that they can be understood by a complete beginner with no programming background.
Before we start with Go, I would like to introduce various tools that are needed for programming and share a few valuable tips.

## **Github**
It is a good idea to create a repository on [github](https://github.com) where you can store your code and share your work with others among other things.
TODO: add on git pull, push, etc...

## **Terminals**
You need a terminal to do any programming work. A terminal is an interface where you can type, edit and execute your programs.
It is a good idea to use tmux, a terminal multiplexer, that allows you to have multiple windows open and to swtich easily between these windows.
If you are using a macbook, use a finder to search for a terminal. Every macbook should have a terminal.
Once you open a terminal, type *tmux attach* to open tmux.
Usually, source code is entered and edited on emacs...

## **Go from start**
The way I see it, Go is a language made up of many packages. To learn more about go, visit [Go website](https://golang.org/).
If you are a complete beginner and feel intimidated by programming (as I have been and still am), I suggest you start exploring in [Go playground](https://play.golang.org/).
There you don't have to worry about terminals.

Here is an example of a simple Go program:
```
package main

import "fmt"

func main() {
fmt.Println("Hello, world!")
}

```
Let me explain in detail each element in the program above.

You always start in main package and import various functions, methods and types from already created packages on Golang.
You need to start precisely with **package main** and not the other way around.
By default, you import a package called **fmt** which allows you to print an output of your program on a terminal, among other things.
The names of all imported packages are in double quotes.
Every main package contains one and only one main function.