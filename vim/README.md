Vim is a modal text editor .
installed almost on every linux distro out there 
vim is powerful ,fast and efficient  

vim has few modes but only 3 are important
- normal mode
- insert mode 
- visual mode

| *Note* : By default when you enter vim you are in normal mode
| if you enter any other mode to go back to the normal mode press <ESC> 
# Motions (on normal mode)
0 to go the start of the line
$ to go the end of the line
% to jump between {} or [] or ()  
w and b jumb by words forwards and backwards
e to jump by words but puts cursor at the end of line
{ and } jump blocks forwards and backwards
f<CHAR> jump to the first in that line <CHAR>
t<CHAR> jump one charachter before the first <CHAR> in that line 
gg tojump to head of the file
G to jump to end of the file
# Actions
@indenation
>> indentation 
<< indent back

### using count with motions

@deletion
x deletes the character under the cursor
daw deletes the word under the cursor
dip deletes a paragraph
dap a paragraph and the whitespace surrounding it
d <motion_command>

exmple:
	dw deletes until the end of the word under the cursor
	dd deletes the entire line
	d$ deletes from cursor postion to the end of the line
	d0 deletes from cursor position to the start of the line
	dgg deletes from cursor position to the start of the line
	dG deletes from cursor position to the end of the line
	db deletes a words from cursor position 
	df<CHAR>
	
	| works also with counts
	d3w deletes 3 words 
	3dd deletes 3 lines	

| deletion also act as copying so when you dd a line you can just paste it with 'p'
@copy and paste
yy copies the entire line
y <motion_command>
	examples:
		
p paste

@replace
r<CHAR> to replace the word under the cursor with a charachter <CHAR>
cc deletes line and puts you in insert mode
c <motion_command>
	examples:
	cw delete word and puts you in insert mode
	c$ deletes from cursor postion to the end of the line and puts you in insert mode
	c0 deletes from cursor position to the start of the line and puts you in insert mode
	cgg deletes from cursor position to the start of the line and puts you in insert mode
	cG deletes from cursor position to the end of the line and puts you in insert mode
	cb deletes a words from cursor position and puts you in insert mode 
	cf<CHAR> deletes to the first occurence of <CHAR> and puts you in insert mode
	
	| works also with counts

R enter replace mode (you can keep replacing until quiting with <ESC>)

@undo and redo
u to undo the last action
CTRL+r to redo 


| Note '.' is used to repeat the last action
| its a very powerful command
Example:
	


# Ways to go into insert mode
i enter insert mode underthe cursor
a move one character forwards and start insert mode  
A enter insert mode at the start of the line
I enter insert mode at the end of the line
o creates a new line under the cursor line and then enters insert mode
O creates a new line above  the cursor line and then enters insert mode


# VISUAL MODE
v <motion command>

CTRL v 

@visual mode + norm ex command


# EX commands
You enter an Ex command by pressiong ':' from normal mode

@substiion
w save a file
e <FILENAME> opens a file in vim 
%s / what to replace / <REPlACE_WITH> / flag
earlier <INT>m 
later <INT>
/ searching
	when match is found:
		n to go to the next occurence
		N to go the previous occurence	

! run an external command
	example: !ls




# The .vimrc (Vim's configuration file)
vim's configuration file


