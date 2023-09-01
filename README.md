# simple_shell
A C program that implements a simple shell/command-line interpreter. It allows users to execute commands, handle background and foreground processes, handle input/output redirection, and pipe commands together. 



## Compile and Run
compile: 
```
gcc -o simple_shell PA1.c
```
run: 
```
./simple_shell
```

## Supported Commands

### basic commands 
`ls`: List files and directories in the current directory.

`pwd`: Print the current working directory.

`echo Hello, World!`: Print the text "Hello, World!".

`date`: Display the current date and time.


### redirection
`ls > files.txt`: Redirect the output of the ls command to a file named files.txt.

`cat < files.txt`: Redirect the contents of the files.txt file as input to the cat command.


### piping
`ls | grep txt`: List files and pipe the output to grep to search for "txt".

`ls | sort`: List files and pipe the output to sort to sort the file names.


### background execution
`sleep 5 &`: Execute the sleep command in the background for 5 seconds.

`ls -R / &`: List files and directories in the root directory in the background.


### job management
`sleep 10`: Execute the sleep command for 10 seconds in the foreground. Press Ctrl+Z to stop it and put it in the background.

`jobs`: Display the list of background jobs.

`bg 0`: Resume the job at index 0 in the background.


### exiting the shell
`exit`: Exit the shell.


