## Shell Script Introduction ##

### WHAT: ###

- Creating  a Script
- Executing a Script
- Best Practice:
    1. always give filename that make sense
    2. executable remove ".sh" extension

* Review download_resource pdf
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

```


