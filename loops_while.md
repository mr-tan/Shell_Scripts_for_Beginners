## Flow Control##

### WHAT: ###

Loops - While

### WHEN: ###

- Execute a command or a set of commands multiple times but you are not
sure how many times
- Execute a command or a set of commands until a specific condition occurs
- Create infinite loops
- Menu driven programs 

Review:
- sleep 2 cmd

---

```bash
# while-loop with comparison operator
a=5
b=10

while [ $a -le $b ]
do 
 echo "Iteration Number: $a"
done

# while-lop with "true" -infinite loop
while true
do 
 echo "I will continue to iterate unless you press Ctrl + C"
 echo "On second though let also rest of 1 second between every iteration"
 sleep 1s
done

```


