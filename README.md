# **notes - draft**
*Notes on learning the Go programming language*

## **Welcome!**
I thought it would be useful to take notes as I am learning Go. These notes are intended for complete beginners like myself. The notes have two tracks, one focusing on the Go language itself and another on the tools associated with Go. 
We will start with a very simple program and gradually build upon it as we learn new concepts. The goal is to eventually have a complex program that does something fun or useful and whose components you understand fully since you have built it from the ground up. To maximize learning, I advise you to type the code and run the program on [Go playground](https://play.golang.org/) as you follow the notes.

You can also play around in the [Tour of Go](https://tour.golang.org/welcome/1).

## **Go from the start**
Go is a language made up of many packages. There are about [40 packages total](https://golang.org/pkg/) in the standard library. You write your program in main package and import relevant packages from the standard library or from a third party. Whenever you import a package, all components of that package (e.g., functions, types, methods) are imported as well. Let's start with a simple program in [Go playground](https://play.golang.org/):
```
package main

import "fmt"

func main() {
    fmt.Println("Hi there, gophers!")
}

```
Let us look at each element above. We start in main package by typing `package main` and importing a package called `fmt` which allows you to print an output of your program onto a terminal. The names of all imported packages are in double quotes. 

Main package contains one and only one main function. To define a function, you type `func` followed by the name of that function, in this case `main`. The name of a function is followed by parentheses as in `func()` inside which you place arguments or inputs for that function. Main function takes no arguments. An output of a function goes right after the closing parenthesis. Main function returns no outputs. The body of a function is enclosed in curly brackets. 

Main function can contain other functions which in turn have their own arguments inside parenttheses (?). You first type the name of the imported package followed by a dot and then the name of the function in that package with the first letter in capital letters as in `fmt.Println`. In general, whenever you use a function or some other element in the imported package, its first letter is in caps. There are several `Print` functions in `fmt`. Here, we used `Println` which allows you to print a line without needing to specify the end of the line (?). If you want to print text as it is you need to enclose it in double quotes. In Go, anything in double quotes is called a string. If you want to print something modified within a string, which is almost always the case in Go, a function `Printf` is used which also come from the package `fmt`, so it is written as `fmt.Printf`. Inside the string, `%v` is used as a placeholder for a specific value which you enter outside the string within the `Printf` function's parentheses. In this case, you need to specify where you want the string to end by entering `\n`. Let's look at an example below. 

First, let us assign a string to a variable. You will need to declare a variable by taking any letter, in this case g for gophers and c for chipmunks, in the following manner `g := "gophers"` which means that you declare a new variable g and assign it to a string "gophers", then declare another variable c and assign it to a string "chipmunks".  

```
package main

import "fmt"

func main() {
    g := "gophers"
    c := "chipmunks"
    fmt.Printf("Hi there, %v.\n", a)
    fmt.Printf("Bye %v.\n", b)
}

```
When you run this function, you should get an output `Hi there, gophers.` and on a line below `Bye chipmunks.`. Note that you need to place a dot before `\n` for it to appear on the same line.

We will keep exploring more functions later. For now, just remember that a function as something that typically takes an input as its arguments and returns an output.

## **On types** ##
Before exploring functions further, let me first introduce types. Broadly speaking, a type is a set of things. For instance, I can have a type `age` which is a set of values for age. These will be in integer form, so we will write it as `type age int`. Types are valuebale because they are defined only ones and can be used in several functions (?). Go has several built-in data types such as integers `uint8` (unsigned 8 bit integer), `uint16` (unsigned 16 bit integer), etc. 


## **On packages and functions** ##
Now, let's add more to our program by importing more packages and adding more functions.

```
package main

import "fmt"

func (a int) int

func main() {
    g := "gophers"
    c := "chipmunks"
    fmt.Printf("Hi there, %v.\n", a)
    fmt.Printf("Bye %v.\n", b)
}

```
If you import more than one package, you enclose them in parentheses. Please note that in [Go playground](https://play.golang.org/) you have an option to automatically import packages. In the program above, we imported "math" package from the standard library which contains basic constants and mathematical functions. 



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


