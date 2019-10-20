# Dmenu Patches
## Script Support
### Description
Allow you to specify a script to dynamicly update the list of entries in dmenu
### Usage
``` sh
dmenu -s "your script"
```
The patch will exxecute the script upon each keystroke 
It will take the list from the standard output of the script (each line an new entry)
The search text entered by the user will be put in the first argument of the script
## Install
``` sh
cd dmenu_path
git branch -b my_dmenu
git apply the_patch.diff
make 
make install
```
