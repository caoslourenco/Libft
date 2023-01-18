<p align="center">
    <img src="https://user-images.githubusercontent.com/18141491/213255060-c287b459-38b5-4404-81af-d31e8c8f8fe3.png">
</p>

<p align="center"> 
    <img src="https://img.shields.io/badge/Status%20-Completed-lightgrey" alt="Grade">
 
</p>

## Libft

This project is about creating a library with useful functions for future projects.


## How to use

- Clone the repository
- Run `make` to compile the library
- Include the header file `libft.h` in your project
- Compile your project with the library `libft.a`

## Mandatory part

- [x] the project must be written in accordance with the Norm
- [x] the project must be written in the C language
- [x] the functions must be prototyped in a header file called `libft.h`
- [x] the functions must be written in separate `.c` files
- [x] the functions must be compiled with the flags `-Wall`, `-Wextra`, and `-Werror`
- [x] the library must be named `libft.a`

### Part 1 - Libc functions

| Function | Description |
| --- | --- |
| ft_isalpha | Checks if the character is an alphabetic character |
| ft_isdigit | Checks if the character is a digit |
| ft_isalnum | Checks if the character is an alphanumeric character |
| ft_isascii | Checks if the character is an ASCII character |
| ft_isprint | Checks if the character is a printable character |
| ft_toupper | Converts a lowercase letter to uppercase |
| ft_tolower | Converts an uppercase letter to lowercase |
| ft_strlen | Calculates the length of a string |
| ft_memset | Fills the first n bytes of the memory area pointed to by s with the constant byte c |
| ft_bzero | Writes n zeroed bytes to the string s |
| ft_memcpy | Copies n bytes from memory area src to memory area dest |
| ft_memccpy | Copies bytes from string src to string dest |
| ft_memmove | Copies n bytes from memory area src to memory area dest |
| ft_memchr | Locates the first occurrence of c (converted to an unsigned char) in string s |
| ft_memcmp | Compares byte string s1 against byte string s2 |
| ft_strlcpy | Copies up to size - 1 characters from the NUL-terminated string src to dst |
| ft_strlcat | Appends the NUL-terminated string src to the end of dst |
| ft_strchr | Locates the first occurrence of c (converted to a char) in the string pointed to by s |
| ft_strrchr | Locates the last occurrence of c (converted to a char) in the string pointed to by s |
| ft_strnstr | Locates the first occurrence of the null-terminated string little in the string big |
| ft_strncmp | Compares not more than n characters. Because strncmp() is designed for comparing strings rather than binary data, characters that appear after a `\0' character are not compared |
| ft_atoi | Converts the initial portion of the string pointed to by str to int representation |
| ft_calloc | Allocates memory for an array of nmemb elements of size bytes each and returns a pointer to the allocated memory |
| ft_strdup | Allocates sufficient memory for a copy of the string s1, does the copy, and returns a pointer to it |


### Part 2 - Additional functions

| Function | Description |
| --- | --- |
| ft_substr | Allocates (with malloc(3)) and returns a substring from the string ’s’. The substring begins at index ’start’ and is of maximum size ’len’ |
| ft_strjoin | Allocates (with malloc(3)) and returns a new string, which is the result of the concatenation of ’s1’ and ’s2’ |
| ft_strtrim | Allocates (with malloc(3)) and returns a copy of ’s1’ with the characters specified in ’set’ removed from the beginning and the end of the string. |
| ft_split | Allocates (with malloc(3)) and returns an array of strings obtained by splitting ’s’ using the character ’c’ as a delimiter. The array must end with a NULL pointer
| ft_itoa | Allocates (with malloc(3)) and returns a string representing the integer received as an argument. Negative numbers must be handled. |
| ft_strmapi | Applies the function ’f’ to each character of the string ’s’, and passing its index as first argument to create a new string (with malloc(3)) resulting from successive applications of ’f’. |
| ft_putchar_fd | Outputs the character ’c’ to the given file descriptor. 
| ft_putstr_fd | Outputs the string ’s’ to the given file descriptor. |
| ft_putendl_fd | Outputs the string ’s’ to the given file descriptor, followed by a newline. |
| ft_putnbr_fd | Outputs the integer ’n’ to the given file descriptor. |

## Exemple

```bash
cc -Wall -Wextra -Werror -I libft.h -L libft.a main.c
```

```c
#include "libft.h"
int main(void)
{
    char *str = "Hello World!";
    ft_putstr_fd(str, 1);
    return (0);
}
```

## To do

- [ ] add more functions
- [ ] add tests
- [ ] add documentation in header file

