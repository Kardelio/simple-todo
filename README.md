# Usage

```
todo 
```
with no arguements... will list out all current todo items with description, priorities and ids...

```
todo "Print out the business report!"
```
will add the todo item to the todo list...
Default priority is NORMAL

```
todo -p HIGH "Print out the business report!"
```
will add the todo item to the todo list with HIGH priority

Priority options (-p):
- h high H HIGH OR 1
- n norm normal N NORM NORMAL OR 2 (**DEFAULT**)
- l low L LOW OR 3

```
todo -e
```
will *EMPTY* the entire todo list **BE CAREFUL!**

```
todo -d 0
```
will complete/delete a todo item with id (imagine as *done*)
<br/>**NOTE:** Can also use -r (imagine as *remove*)

```
todo -d print
```
will complete/delete a todo item where the string matches (imagine as *done*), uses regex pattern matching to find all tickets that contain that string in the description.
<br/>**NOTE:** Can also use -r (imagine as *remove*)