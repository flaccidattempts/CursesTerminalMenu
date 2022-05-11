# CursesTerminalMenu
A simple Template for Creating a reactive Curses Menu in windows terminal 10-11







[Funamental Curses Knowledge](<#fundamental-windows-curses-knowledge> "New to Curses")

[Quick Overview](<#description> "A quick description of the script")

[Customizing your menu](<#changing-highlight-colors> "New to Curses")




## Fundamental Windows Curses Knowledge

1. You can not effectivly test the graphical components of your curses program in an IDE. Windows Console Host Only.
2. Always make an exit for your code while using the Curses module. You can get stuck pretty fast.
3. To install curses on windows --> pip install windows-curses
4. This is different from importing it into your py file --> import curses


## Description

If you have questions about this script i can go into further details.

Use the up and down arrows to navigate the Menu and enter to choose your selection.

Title, subtitle, options and slots are all customizable. 


## Changing Highlight Colors

Line 21 : Using the

``````python
curses.init_pair(curses.COLOR_"text color in all caps", curses.COLOR_"background color in all caps")
``````

## Changing Normal Text Colors

Line 23:

````python
self.normal_color = curses.A_NORMAL
````

This line controls the menu options that are not selected. You could change this to an intialized pair or whatever curses attribute you desire.

## Changing Menu Title

To change title go to Line 106:

````python
  menu = {'title' : 'your title goes here',
````

## Changing Description

Navigate to line 108...

`````python
'subtitle' : 'your subtitle description here'
`````

## Changing Menu Options

Navigate to line 110:

````python
option_1 = {'title' : 'Menu option title goes here'
````

you can change this text to suit your needs
  
## Adding new Options

### step 1.
 Navigate to Line 109:
 
 create a new set variable like so
 ````python
  option_2 = {'title' : 'your option title here',
    'type' : 'selected action command here',
    'command' : 'Command to execute here'}
  ````
### step 2.

Add the set variable to your list of sets like so

line 118:

`````python
menu['options'] = [option_1, option_2]
`````


  
  
  
 
