# Now we're getting into real deal
We're introduced to some of the most used commands in Linux:
- ``cp`` → Copy files and directories
- ``mv`` → Move or rename files and directories
- ``mkdir`` → Create directories
- ``rm`` → Remove files and directories 
- ``ln`` → Create hard and symbolic links

## Some cabbeats
We are told that **this tasks can be more easily done using the GUI**.

## Why use this commands?
The answer relies on Power and flexibility. While it is easy to perform simple file manipulations with a Graphical File Manager, complicated tasks can be easier with the command line programs. 

For example, if we want to copy a bunch of files that are only HTML from one place to another we would do this. 

```bash
cp -u *.html destination
```

## Wildcards

You might wonder what are the ``*`` or ``.`` signs. Well, these are special characters that are called wildcards. Using wildcards (which are also known as **globbing**) allow us to select filenames based on patterns of characters.


| Wildcard | Matches | Examples |
| :--- | :--- | :--- |
| `*` | Matches any character including none | `file*` matches `file`, `file1`, and `file.txt`. <br> `*.txt` matches all `.txt` files. |
| `?` | Exactly one single character. | `file?.txt` matches `file1.txt`, `file2.txt`, etc. |
| `[...]` | Any single character that is a member of the specified set. | `[abc]file` matches `afile`, `bfile`, or `cfile`. |
| `[!...]` or `[^...]` | Any single character that is not a member of the specified set. | `[!a-z]file` matches any file that does not start with a lowercase letter. |
| `[[:class:]]` | A specific character class (e.g., `[:digit:]`, `[:alpha:]`, `[:lower:]`, `[:upper:]`). | `*[[:lower:]]` matches any file ending in a lowercase letter. |

### Wildcard examples

| Pattern | Matches |
| :--- | :--- |
| `*` | All files |
| `g*` | Any file beginning with *g* |
| `b*.txt` | Any file beginning with *b* followed by any characters and ending with *.txt* |
| `Data???` | Any file beginning with *Data* followed by exactly three characters |
| `[abc]*` | Any file beginning with either an *a*, a *b*, or a *c* |
| `BACKUP.[0-9][0-9][0-9]` | Any file beginning with *BACKUP.* followed by exactly three numerals |
| `[[:upper:]]*` | Any file beginning with an uppercase letter |
| `[![:digit:]]*` | Any file not beginning with a numeral |
| `*[[:lower:]123]` | Any file ending with a lowercase letter or the numerals *1*, *2*, or *3* |