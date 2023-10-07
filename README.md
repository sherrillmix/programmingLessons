# Programming intro
## General
* Spaces are a pain in filenames. Try to avoid
* Press up to get back to previous command
* Watch out for incomplete commands e.g. `setwd("SOME_DIRECTORY)` notice the missing `"` on the right. The command line will look something like:
  ```
  > setwd("SOME_DIRECTORY)
  + 
  ```
  The `+` sign instead of a `>` is an indication that R is waiting for additional input.
* The `>` (or similar) at the start of lines is used to indicate the terminal/R is waiting for a command. Do not type `>` at the start of lines when inputting code.


## Bash
Available using Terminal program on Macs or Terminal tab in RStudio
* `ls` : list files in a directory
* `rm FILETNAME_TO_DELETE` : remove a file in a directory. This is permanent, be very careful

## R
* `x=5` : assign x as 5
* `x^2` : square variable x 
* `getwd()` : show current directory
* `setwd("DIRECTORY/TO_GO_TO")` : change the current directory
* `list.files()` : show files in current directory
* `source("FILE_CONTAINING_R_CODE")` : input all the code in a file into R. This could allow someone to do bad things so don't do it on files you haven't written
* `dir.create("DIRECTORY/TO_CREATE")` : create a directory
* `?FUNCTION_NAME` e.g. `?dir.create` : get help on a function
