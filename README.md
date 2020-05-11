### What is this repository?

You are in a little repository about linux. Go to [master](https://github.com/renanzulian/linux) and let know what I'm doing here.

## Section 1 - GNU and Unix commands


### Working on Command line

The terminal is probabily the first things that peoples remember when the subject is Linux. The terminal is basicly a interface to execute commands on linux. The correct term of this interface is **shell**. All Operational System from linux provides some type of shell (usually is bash). You can find many types of shell like zsh, sh, csh and much more. Then you only need to keep on your mind that *we use the shell to execute our commands.*

On linux shell you can have two types of commands:

1. Internal command
    
    Is an own command of shell. On bash for example you can have `cd` command to change the working directory of shell. How do I know that `cd` is a own command of shell? Easy only use command the command `type`.
    
    ![type cd](./assets/type_cd.png)

    try ever command that you know using `type [command]` and discover what type is your command!

2. External command

    This commands can be installed on your machine and they are independent of your shell. For example when you install vim you **will can** use the command `vim` to edit some text file. But you only will may use this command if your shell knows where the binary is. It means that independent of your external command you need to provide the **PATH** of them to your shell. The linux environment variable PATH is used to shell find where is your binaries. Let's find where is our vim binary:

    ![type vim](./assets/type_vim.png)

    Very nice the command also is on hash (on memory) and our shell knows this command. It means the command is on PATH an we can check it using another good command `echo`.

    ![echo path](./assets/echo_path.png)

    All directories are separated with by colon and whe can find the vim's directory **/usr/bin** on the path. Whether the directory isn't on path the shell would output "bash: vim: command not found".

    If you wanna execute some script or binary that isn't on your path you only need to type down it's absolute path or use `./[nome of the script/binary]` on folder that the content be.



shell bash

echo

three types of commands

interno(do bash) externos(in path) externo(not in path)

pwd

ls

cd

abosolute path and relative path

path