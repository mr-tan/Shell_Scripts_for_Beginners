## Flow Control##

### WHAT: ###

Loops - For

### WHEN: ###

- Execute a command or a set of commands many times
- Iterate through files
- Iterate through lines within a file
- Iterate through the output of a command

---

```bash
# Loop - For Syntax
for mission in lunar-mission jupiter-mission saturn-mission
do
# bash /home/bob/create-and-launch-rocket $mission
  create-and-launch-rocket $mission
done

# Loops from text file
for mission in `cat mission-names.txt`
do 
  create-and-launch-rocket $mission
done

# Loops from text file (best practice)
for mission in $(cat mission-name.txt)
do 
  create-and-launch-rocket $mission
done

# Append text in loop
for mission in $(cat mission-name.txt)
do 
  create-and-launch-rocket mission-$mission
done

# Looping specific number of times
for mission in {0..100}
do 
  create-and-launch-rocket $mission
done

# Loop with initialization eg. traditional
for (( mission=0; mission <= 100; mission++ >))
do
  create-and-launch-rocket mission-$mission
done

# Ex_01
for file in $(ls)
do
 echo Line count of $file is $(cat $file | wc -l)
done

# Ex_02
for package in $(cat install-packages.txt)
do 
  sudo apt-get -y install $package
done

# Ex_03
for server in $(cat servers.txt)
do 
 ssh $server "uptime"
done

```


