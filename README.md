# TimberScript
Cheat Engine Assembly script written in lua that will play until the 32-bit integer limit

Tested 26501 cuts before quitting
Integer limit will take approximately 2.27 years on the machine the script was tested on as it ran at 30 cuts per second

###Implementation Details###
This script uses CheatEngine's memory enumeration in order to consistently find the array offset that stores the treepart.

These treeparts contain data on which side the limb is on.

The script reads this data and executes a keypress on the opposite side of the next limb everytime the memory address is updated 
i.e. the next treepart shifts down.

################################

Note:This was only tested on one machine, performance may vary depending on Timberman's running framerate.
