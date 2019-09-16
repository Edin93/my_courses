# Expansion
1. the shell expands any qualifying characters, before the command execution.
2. pathname expansion: is the mechanism on which wildcards work.
3. tilde expansion (~some_user):
* WHEN USED AT THE BEGINNING OF A WORD, it expands into the home directory of the given user.
* when there's no user, then the home directory of the current user.
4. arithmetic expansion: $(( arithmetic_expression )):
* arithmetic expansion supports only integers (whole numbers, no decimals).
5. brace expansion { brace_expression } :
* it can create multiple text strings from a patter containing braces.
* brace expression can contain either:
  - a comma separated list of strings. ex: {a,b,c}
  - a range of integers of single characters. ex:  {1..8}, {a..Z}, {z..a}
  - a single character.
  - brace expansion may be nested. ex: img{a{1,2,3}, b{1,2,3}}.jpg
6. parameter expansion:
* ex: echo $param

# IMPORTANT:
===>  if you mistype a pattern, the expansion will not take place and the echo command will simply display the mistyped pattern. With parameter expansion, if you misspell the name of a variable, the expansion will still take place, but will result in an empty string.

# Command Substitution
* syntax: $(command_to_substitute)
* command substitution allows us to use the output of a command as an expansion.
* ex: echo $(ls), ls -l $(which cp)
* In older shell programs, we can substitute the commands with backquotes `command_to_substitute` (it's supported in bash).

# Quoting
* the shell provides a mechanism called quoting to prevent unwanted expansions.
### Double quotes
* special characters inside double quotes lose their special behavior, the execptions are: $, \ and ` (back-quote) ----> meaning paramater expansion, arithmetic expansion and command substitute are still carried out.
### Single quotes
* single quotes suppress all expansions.

# Variables
* shell variables are in uppercase characters by convention.
### global variables:
- global variables or environment variables are available in all shells.
### local variables:
- local variables are only available in the current shell.

# 4 types of variables:
* string
* integer
* constant
* array

# Shell initializatin files:
## /etc/profile.d Directory:
* a directory containing files configuring system-wide behavior of special programs.
## /etc/profile File:
* a configuration file that sets some basic shell environment variables.
