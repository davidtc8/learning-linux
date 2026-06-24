# Useful Commands

- ``ls`` → List Directory Contents
- ``pwd`` → Print Name of current working directory
- ``cd`` → Change directory
- ``file`` → Determine file type
- ``less`` → View File Contents

## Table 3-1: Common ``ls`` Options

As described in the book, the ``ls`` command has many possible options. 

| Option | Long Option | Description |
| :--- | :--- | :--- |
| **-a** | `--all` | Lists all files, including hidden files (those starting with a period). |
| **-A** | `--almost-all` | Lists all files except for `.` (current directory) and `..` (parent directory). |
| **-d** | `--directory` | Lists the directory itself rather than its contents (used with `-l` to see directory permissions). |
| **-F** | `--classify` | Appends an indicator character to the end of each listed name (e.g., `/` for a directory). |
| **-h** | `--human-readable` | Displays file sizes in human-readable terms (e.g., K, M, G) instead of bytes; requires `-l`. |
| **-l** | *None* | Displays results in long-listing format, showing permissions, owner, size, and timestamp. |
| **-r** | `--reverse` | Reverses the sorting order of the results (alphabetical by default). |
| **-S** | *None* | Sorts the output results by file size. |
| **-t** | *None* | Sorts the output results by modification time. |

## What we've learned?
In this chapter I've learned how to use the ``less`` command, which opens a VIM view in the command line, in there I can view the file I'm trying to read (might be ready to use NeoVim? XD).

## Personal thoughts
The more I come to knowing the terminal, the less I want to depend on the UI.