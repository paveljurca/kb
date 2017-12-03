```sh
find -maxdepth 1 -type d -exec ls -di {} \;|awk ' /reg_exp/ { print "DIR " $2 " = " $1 }'

grep -Eo "^[^:]*" < /etc/passwd (print all users on your linux machine)

grep -Ev "^(#|REM|'|\/\/|\/\*)" < $1 (erase all one-line comments)

grep -E "^([^#])" < $1 (all lines except one-line comments and empty lines)

echo "606-234-854"|grep -E "^[0-9]{3}-[0-9]{3}-[0-9]{3}\b" (accepts only 6-digit number)

echo "` <$0`" OR echo "`cat $0`" (Echoes the script itself to stdout)

if ! [[ $USER = "root" ]]; then echo "you are not super-user jockey, sry"; fi

var=`-name`;a="*sh";find " $var" $a 2>/dev/null (option substitution --> really interesting!!)

echo "$var"|sed -r "s/(^[[:space:]]+|[[:space:]]+$)//g" (sed -r means extended support for reg expressions)

continue (skip to the next lap of loop)

echo "hello_world">file.$RANDOM (random file creating process)

g="0000017";echo ${g:$[ ${#g}-3 ]} (returns 3 last chars offset at the end)

sed '1d;$d' file.txt	(1 means first line, d means delete, ; separator, $ means last line)

while ... do ... done <<< "$OUTPUT"

while ... do ... done < <(echo "$OUTPUT")
```
