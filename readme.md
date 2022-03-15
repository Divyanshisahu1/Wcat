# Build WCAT commands


It is used to display or make a copy content of one or more files in the terminal 

General Syntax:
node wcat.js [options] [filepaths]
option to remove big line break (-s)
option to add line number to non empty lines (-b)
option to add line numbers to all lines (-n) 
option to create new file (-c)

Commands:
<br>
<br>1- node wcat.js filepath => displays content of the file in the terminal  ✔
<br>2- node wcat.js filepath1 filepath2 filepath3... => displays content of all files in the terminal in (contactinated form) in the given order. ✅ 
<br>3- node wcat.js -s filepath => convert big line breaks into a singular line break
<br>4- node wcat.js -n filepath => give numbering to all the lines
<br>5- node wcat -b filepath => give numbering to non-empty lines
<br>6- node wcat -c filepath =>it creates a new file in given path and write data which is passed in second arguement and if given file already exist,it overwrites the data in that file so we need to care of that.
<br>NOTE-We can mix and match the options.

Edge cases:
<br>
<br>
1- If file entered is not found then it gives file does not exist error. ✅ <br>
2- -n and -b are 2 options which are mutually exclusive so if user types both of them together only the first enter option should work.<br>
3- -s and any or both -n and -b present then -s will be executed first and then -n and -b according second rule 
