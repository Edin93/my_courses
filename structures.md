# Structure:
* A structure is a user defined data type available in C that allows to combine data items of different kinds.
## Structure declaration:
* You can define a structure in the globa scope of your program.
* You can declare elements of your structure in its scope.
## Example:
struct User
{
char *name;
char *email;
int age;
}

int main(void)
{
struct User user;
return (0);
}

## Structure definition by wikipedia:
* A struct in the C programming language (and many derivatives) is a composite data type (or record) declaration that defines a physically grouped list of variables under one name in a block of memory, allowing the different variables to be accessed via a single pointer or by the struct declared name which returns the same address. The struct data type can contain other data types so is used for mixed-data-type records such as a hard-drive directory entry (file length, name, extension, physical address, etc.), or other mixed-type records (name, address, telephone, balance, etc.).