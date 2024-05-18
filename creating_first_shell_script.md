## Shell Script Introduction ##

### WHAT: ###

- Creating  a Script
- Executing a Script
- Best Practice:
    1. always give filename that make sense
    2. executable remove ".sh" extension
    3. design script to be re-usable
    4. command line input as pass in value

* Review download_resource pdf

Variables:
- "{}" usage ?
- $(rocket-status $mission_name) ?
- read -p "enter mission name:" mission_name

Arithmetic Operations:
- must review
---

```bash
# Run shell script
[~]$ bash create-and-launch-rocket.sh

# Run shell script
[~]$ create-and-launch-rocket

# Command not found error msg
[~]$ echo $PATH
/usr/local/sbin:...

# Fix error msg by adding home path
[~]$ export PATH=/usr/local/sbin:/home/michael

# Better way of home path
[~]$ export PATH=$PATH:/home/michael

# Command Line Arguments
# argument $0
[~]$ create-and-launch-rocket

# argument $1
[~]$ create...saturn-mission

# Arithmetic Operations
[~]$ expr 6 + 3
[~]$ expr 6 / 3
[~]$ expr 6 * 3

# Using variables in arithmetic operations
[~]$ A=6
[~]$ B=3
[~]$ expr $A + $B

# Using parenthesis in arithmetic operations
# Also for incrementor
[~]$ echo $(( A + B ))

# Arithmetic operation w/ float points
[~]$ echo $A /$B | bc -l

```


