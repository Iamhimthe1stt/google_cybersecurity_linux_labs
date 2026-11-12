# Lab 2: Get Help in the Command Line

## Objective
Use Linux help tools to learn what commands do and to find the right command when I don't remember its name.

## Commands used
```bash
whatis cat                      # one-line description of cat
man cat                         # full manual page (found -n, --number)
apropos -a first part file      # search by keyword (found head)
man useradd                     # full manual page (found -e, --expiredate)
whatis rm                       # remove files or directories
whatis rmdir                    # remove empty directories only
apropos -a create new group     # search by keyword (found groupadd)
```

## What I learned
| Tool | What it does | When to use it |
|---|---|---|
| `whatis` | One-line description of a command | Quick reminder of what a command does |
| `man` | Full manual with every option | Need details about options |
| `apropos` | Searches manual descriptions by keyword | Don't remember the command name |

- `cat -n` numbers all output lines.
- `useradd -e` sets an account expiration date, useful for temporary accounts.
- `rm` removes files or directories, while `rmdir` only removes empty directories.
- `head` returns the first part of a file.
- `groupadd` creates a new group.

## Takeaway
Analysts won't know every command, so knowing how to look them up quickly is a core skill. In the manual, Space shows the next page and `q` exits.

## Screenshots
![whatis and man cat](screenshots/01-whatis-and-man-cat.png)
![man cat end](screenshots/02-man-cat-end.png)
![apropos finds head](screenshots/03-apropos-head.png)
![man useradd](screenshots/04-man-useradd.png)
![whatis rm and rmdir](screenshots/05-whatis-rm-rmdir.png)
