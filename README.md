# TurtleScript
A parser and renderer that reads TurtleScript commands from a TurtleScript file (.tsf) and then performs the specified actions on screen.

![demo](https://github.com/Nytra/TurtleScript/blob/master/demo1.gif)

Just a demonstration of a turtle drawing my name onto the screen.

![demo](https://github.com/Nytra/TurtleScript/blob/master/yeah_it_supports_comments.PNG)

The TurtleScript code for the above drawing.

![Random TurtleScript](https://github.com/Nytra/TurtleScript/blob/master/random.PNG)

The program is capable of generating random TurtleScript files with a specified number of actions. The program ensures that the turtle does not leave the confines of the screen.

---

## Intro

TurtleScript is a name that I just made up for a scripting language meant for controlling turtles (little nasties that algorithmically make a mess on the screen).

The idea for this program came from a book called "The Pragmatic Programmer" by Andrew Hunt and David Thomas (page 63 exercise 5)

The exercise just states that you must implement a *parser* for the scripting language- but, of course, I couldn't just stop there. 

This program supports multiple colours(3!), navigation in 4(!) directions, and pen up/down commands. You could draw anything from your wildest imagination.

---

## Using TurtleScript

Place your TurtleScript files in the same directory as the main program. Upon execution, the program will ask you to input the name of a TurtleScript file. Once you have done so, the program will begin drawing your beautiful artistic masterpiece on the very screen before your eyes :D

### Syntax:

Most TurtleScript commands come in the form of an uppercase letter, followed by a space, followed by a number.

Example: `"N 12"`

Some commands do not take an argument, so for them you would just type the uppercase letter.

Example: `"D"`

The parser supports comments, but only at the end of the line.

Example: `"N 4 # this is a comment"`

The following TurtleScript code will draw a hollow square on screen.

```
P 0 # select red pen
D 	# pen down
W 5	# go west (left) 5 positions
N 5	# go north (up) 5 positions
E 5	# go east (right) 5 positions
S 5	# go south (down) 5 positions
```