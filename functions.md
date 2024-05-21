## Functions ##

### WHAT: ###

Functions

### WHEN: ###

- Break up large script that performs many different tasks:
    - Installing packages
    - Adding users
    - Configuring firewalls
    - Perform Mathematical calculations

- Best Practice:
    - always develop scripts in a modular re-usable way using functions
    - avoid duplicate code
    - use arguments/parameters to pass in variables
---

```bash
# Function syntax
function add(){
  echo $(( $1 + $2 ))
}

sum=$( add 3 5 )

```


