# Adding A Custom `bin` Directory

In this exercise we're going to modify your shell configuration to allow you to
create and run custom shell commands. To do this you will need to:

1. Add a directory to your `$path`
2. Put executable files in that directory

_If you want to push yourself in this exercise, skip the guide below and see if
you can complete this exercise by just googling how to do it._

## Completion Criteria

You've completed this exercise when:

- You have a directory somewhere on your system dedicated to custom shell
commands. I recommend `~/bin`
- There is at least one executable file within that directory
- You can run a custom command from anywhere in a new terminal window

## Search Terms

```
os x terminal create directory
os x chmod
os x chmod make executable
os x add directory to path
```

## Resources

<!-- not sure why this didn't work
- [Shebang_(Unix)](https://en.wikipedia.org/wiki/Shebang_(Unix))
-->
- <a href="https://en.wikipedia.org/wiki/Shebang_(Unix)">Shebang_(Unix)</a>

## Step By Step Guide


___Note:__ This guide assumes you're using BASH and not ZSH_

1. Create a directory in your home directory called `bin`
0. `touch` a file in that directory called `saymyname`
0. Use the `chmod` command to make this file executable
0. Put `echo $USER` inside of the `saymyname` file
0. Run `~/bin/saymyname` and make sure it outputs your system username
0. Edit your `~/.bashrc` file (if it doesn't exist, create it)
0. Add the line `export PATH="~/bin:$PATH"` to your `.bashrc`
0. Open a new terminal
0. Run `saymyname`
