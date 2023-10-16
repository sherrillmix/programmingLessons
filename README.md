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
### Day 1
* `x=5` : assign x as 5
* `x^2` : square variable x 
* `getwd()` : show current directory
* `setwd("DIRECTORY/TO_GO_TO")` : change the current directory
* `list.files()` : show files in current directory
* `source("FILE_CONTAINING_R_CODE")` : input all the code in a file into R. This could allow someone to do bad things so don't do it on files you haven't written
* `dir.create("DIRECTORY/TO_CREATE")` : create a directory
* `?FUNCTION_NAME` e.g. `?dir.create` : get help on a function

### Day 2
* `1:10` : make a range of numbers 1 through 10
* `c(1,3,5)` : make a "vector" (collection) of the numbers 1, 3, 5 (`c` stands for combine)
* `LETTERS` : a constant builtin variable in R providing a vector of the 26 upper case letters in order
* `LETTERS[1:10]` : select the first ten letters
* `LETTERS[c(1,3,5)]` : select the first, third and fifth letters
* `'some string'` or `"some string"` : use `'` or  `"` to suround strings (text or letters). Failing to do this will result in R failing to parse the command (e.g. `x=some string` produces `Error: unexpected symbol in "x=some string"`) or looking for a variable that does not exist (e.g. `x=some` produces `Error: object 'some' not found`)
* `history()` : display recently run commands
* `LETTERS=='B'` : return a TRUE/FALSE vector where TRUE indicates which elements are equal to B
* `table(x)` : count the number of occurences of items in `x`
* `x$lamp` : access the `lamp` column (if data.frame) or item (if list) in `x`
* `x[1,]` : access the first row of `x` (where `x` is a data.frame)
* `x[1:5,'520nm']` : access the first 5 values in the "520nm" column in `x` (where `x` is a data.frame)
