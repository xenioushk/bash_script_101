# A simple bash script guideline for beginner

## Create first bash script

Create a file and named it **mybash.sh**. Bash script must contain **.sh** extension. Now, open that file in any editor and add this codes.

```bash
#!/bin/bash
echo "I Love Bash Scripting"
```

## Print anything

```bash
echo "Add your text here"
```

## Define a variable

```bash
rootDir="/Applications/XAMPP/xamppfiles/htdocs"
```

## Concate string with a variable

```bash
rootDir="/Applications/XAMPP/xamppfiles/htdocs"
wooPlugDir=$rootDir"/dev.woo.plug"
```

## Print a variable

```bash
latestWpBakery="7.9"
echo $latestWpBakery  #It will print 7.9
```

## Arithmatic comparision

```bash
# -lt 	<
# -gt 	>
# -le 	<=
# -ge 	>=
# -eq 	==
# -ne 	!=
```

## String comparison

```bash
# = 	equal
# != 	not equal
# < 	less than
# > 	greater than
# -n s1 	string s1 is not empty
# -z s1 	string s1 is empty
```

## Declare an array

```bash
# Declare all plugins array
allPlugins=("baf" "bnm" "bpvm" "bkbm" "bpm");
```

## For loop

```bash
# Declare all plugins array
allPlugins=("baf" "bnm" "bpvm" "bkbm" "bpm");
for i in ${!allPlugins[@]};
do
    # Fetch the current plugin name
    plugin=${allPlugins[$i]}
    echo $plugin
done
```

## Function

```bash
function updateNow(){

  # Print param 1
  echo $1
  # Print param 2
  echo $2
}

#Call the updateNow function
updateNow "param 1" "param 2"
```

## Sleep function

```bash
# Sleep the program for 3 seconds
sleep 1
```
