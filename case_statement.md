## Case Statements ##

### WHAT: ###

Case Statements

### WHEN: ###

- Clean logic in instances there are multiple if-else statements

---

```bash
# Case Statement Syntax
while true
do
 echo "1. Shutdown"
 echo "2. Restart"
 echo "3. Exit Menu"
 read -p "Enter your choice: " choice

 case $choice in
  1) shutdown now
  ;;
  2) shutdown -r now
  ;;
  3) break
  ;; 
  *) continue
  ;;
 esac

done

```


