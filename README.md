# 👷‍♀️ Pipex

<div align=center>

  ![badge](https://raw.githubusercontent.com/angelamcosta/angelamcosta/main/42_badges/pipexe.png)
  
  [![forthebadge](https://forthebadge.com/images/badges/made-with-c.svg)](https://forthebadge.com) [![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](https://forthebadge.com)
</div>

## Table of Contents

- [Introduction](#introduction)
- [Mandatory part](#mandatory-part)
- [Bonus part](#bonus-part)
- [Tasks](#tasks)

## Introduction

This project will let you discover in detail a UNIX mechanism that you already know
by using it in your program.

The subject of the project can be found in [this link](https://raw.githubusercontent.com/angelamcosta/pipex/main/en.subject.pdf).

## Mandatory part

Your program will be executed as follows:

```shell
$> ./pipex file1 cmd1 cmd2 file2
```

It must take 4 arguments:
- file1 and file2 are file names.
- cmd1 and cmd2 are shell commands with their parameters.
It must behave exactly the same as the shell command below:

```shell
< file1 cmd1 | cmd2 > file2
```

Your project must comply with the following rules:
- You have to turn in a Makefile which will compile your source files. It must not
relink.
- You have to handle errors thoroughly. In no way your program should quit unexpectedly (segmentation fault, bus error, double free, and so forth).
- Your program mustn’t have memory leaks.
- If you have any doubt, handle the errors like the shell command:

```shell
< file1 cmd1 | cmd2 > file2
```

### Bonus part

You will get extra points if you:
- Handle multiple pipes.
This:

```shell
$> ./pipex file1 cmd1 cmd2 cmd3 ... cmdn file2
```

Should behave like:

```shell
< file1 cmd1 | cmd2 | cmd3 ... | cmdn > file2
```

- Support « and » when the first parameter is "here_doc".

This:

```shell
$> ./pipex here_doc LIMITER cmd cmd1 file
```

Should behave like:

```shell
cmd << LIMITER | cmd1 >> file
```

## Tasks

- :white_large_square: Mandatory part (ongoing)
- :white_large_square: Bonus part (ongoing)
