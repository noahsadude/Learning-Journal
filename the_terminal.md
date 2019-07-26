## The terminal

First, a few commands:
- `cd`: change directory (`cd ..` moves you up a directory, `~` will take you to root)
- `ls`: list all public files/folders (`-a` flag will show hidden files - aka "dotfiles")
- `pwd`: print working directory (where am i?)
- `touch`: create a file
- `mkdir`: create a directory
- `rm`: remove a file (`-r` flag will remove a directory; rm -rf will remove a directory with fire - do not use fire )
- `cat`: show contents in a file
- `file [path]`: specifies the file type

A few key points:
- Don't want to explicitly state which file/folder you want to access? Just press tab- the terminal will do the rest
- There are many, many different flags for each of the above commands. Use `info [command]` to delve into the spells-er, commands, more.
- Remember that you can always specify an absolute path after cd, whereever you are, and you'll arrive directly there
- Because POSIX systems are extensionless, a .txt file might not be what you think it is. `file` is your friend.
- The terminal is case sensitive. You have been warned.
