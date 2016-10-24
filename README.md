#Pipeify

Pipe stuff into a program that does not accept input from stdin (firefox,
libreOffice, etc) by creating a tmpfile. The script itself is shorter
than this README :)

##Requirements

`bash` and standard Linux coreutils type stuff like `cat`. Probably would work
on other POSIX-compliant systems

##Installation

It's a tiny little script. Put it in your `$PATH` somewhere.

##Usage

`pipeify` will simply run the program you specify, with the arguments you
specify, with the name of the tempfile as the final argument.

```
<your_pipeline_here> | pipeify firefox
```

```
<your_pipeline_here> | pipeify libreoffice --calc
```
