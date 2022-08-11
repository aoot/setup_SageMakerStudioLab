# README!!!
These are scripts and stuff I use to setup my Amazon SageMaker Studio Lab environment.

The actual environmental variable script is git-ignored.

## Set up the environment variable in the parent process
[Source](https://askubuntu.com/questions/53177/bash-script-to-set-environment-variables-not-working)
I have been experiencing issues where the bash set environment variable does not show up when I execute echo.
Upon the SO post above, it is because `export` runs the variable setting command in the child command.

Solution:
Use `source` or `.` to run the script, instead of `bash`.

## Difference between `%` ipython magic command vs `!`
- `!` creates a terminal subprocess

## Env variables not loaded through bash from terminal not showing up in Jupyter Notebook
- This might be that the terminal and ipython are running on separate processes.
