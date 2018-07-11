# Usage

```
todo 
```
with no arguements... will list out all current todo items with description, priorities and ids...

```
todo -h
```
Will print out the help information for this program

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
todo -t TODAY "Print out the business report!"
```
will add the todo item to the todo list with a Tag of TODAY

Tags can be any sort string, this will allow you to identify special items quickly

```
todo -e 1
```
will *EDIT* the selected todo item with the matching ID

It will trigger a user interactive edit, where the user can change the description and the priority when prompted.

```
todo -r
```
will *REMOVE ALL* the entire todo list **BE CAREFUL!**

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
