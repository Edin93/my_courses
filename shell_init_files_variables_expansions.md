# Expansion
1. the shell expands any qualifying characters, before the command execution.
2. pathname expansion: is the mechanism on which wildcards work.
3. tilde expansion (~some_user):
* WHEN USED AT THE BEGINNING OF A WORD, it expands into the home directory of the given user.
* when there's no user, then the home directory of the current user.

- arithmetic expansion: $(( arithmetic_expression )):
