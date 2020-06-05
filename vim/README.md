# VIM

Vim is a modal text editor, open-source and installed almost on every linux distro out there.

Vim is powerful, fast and efficient due to its ability to seprates the idea of actions,moving and editing of a file.

Vim has 6 modes but these 3 are the most important:

- **Normal** mode
- **Insert** mode 
- **Visual** mode

> **Note** : By default when you enter vim you are in **NORMAL** mode
>$ -  if you enter any other mode to go back to the **NORMAL** mode press <button>ESC</button>

## NORMAL MODE
## Motions
Moving in vim is done mainly in **NORMAL** mode.  

Here are the most used motions keybinding :   

**`0`** to go the start of the line  

**`$`** to go the end of the line  

**`%`** to jump between {} or [] or ()   

**`w`** and b jumb by words forwards and backwards  

**`e`** to jump by words but puts cursor at the end of line  

**`{`** and **`}`** jump blocks forwards and backwards  

**`f<CHAR>`** jump to the first `<CHAR>` in that line 

**`t<CHAR>`** jump one charachter before the first <CHAR> in that line   

**`gg`** tojump to head of the file

**`G`** to jump to end of the file
### using count with motions
- vim support

## Actions
### Indentation
**`>>`** indentation  
**`<<`** indent back

### Deletion
**`x`** deletes the character under the cursor  
**`daw`** deletes the word under the cursor  
**`dip`** deletes a paragraph  
**`dap`** deletes a paragraph and the whitespace surrounding it  
**`d`** <motion_command>  

<ins>Examples:</ins>  

**`dw`** deletes until the end of the word under the cursor  
**`dd`** deletes the entire line  
**`d$`** deletes from cursor postion to the end of the line  
**`d0`** deletes from cursor position to the start of the line  
**`dgg`** deletes from cursor position to the start of the line  
**`dG`** deletes from cursor position to the end of the line  
**`db`** deletes a words from cursor position  
**`df<CHAR>`** deletes from cursor until character `<CHAR>`  
>works also with counts  

**`d3w`** **d**eletes **3** **w**ords   
**`3dd`** deletes 3 lines	

> deletion also act as copying so when you dd a line you can just paste it with 'p'  

### Copy and paste
**`yy`** copies the entire line  
**`p`** paste  
**`y`** <motion_command>  
* <ins>Examples</ins>:   
	**`y$`** copies to the end of the line  
	**`yG`** copies to the end of the file  
	**`ygg`** copies to the beggining of the file  
	**`yw`** copies from the cursor position until the end of the word under the cursor  
	**`yaw`** copies the entire word under the cursor  

### Replace

**`r<CHAR>`** to replace the word under the cursor with a character `<CHAR>`   
**`cc`** deletes line and puts you in insert mode    
**`c`** <motion_command>
* <ins>Examples:</ins>   
	**`cw`** delete word and puts you in insert mode  
	**`c$`** deletes from cursor postion to the end of the line and puts you in insert mode  
	**`c0`** deletes from cursor position to the start of the line and puts you in insert mode  
	**`cgg`** deletes from cursor position to the start of the line and puts you in insert mode  
	**`cG`** deletes from cursor position to the end of the line and puts you in insert mode  
	**`cb`** deletes a words from cursor position and puts you in insert mode   
	**`cf<CHAR>`** deletes to the first occurence of `<CHAR>` and puts you in insert mode  
	
	>  works also with counts  

	**`3cc`** deletes 3 lines and enters insert mode

**`R`** enters replace mode (you can keep replacing until quiting with <button>ESC</button>)  

### Undo and redo
**`u`** to undo the last action  
**`CTRL+r`** to redo  
**`.`** is used to repeat the last action  
	

## INSERT MODE
* insert mode is where you change text inside of the file you opened

**`i`** enter insert mode underthe cursor    
**`a`** move one character forwards and start insert mode    
**`A`** enter insert mode at the start of the line  
**`I`** enter insert mode at the end of the line  
**`o`** creates a new line under the cursor line and then enters insert mode  
**`O`** creates a new line above  the cursor line and then enters insert mode


# VISUAL MODE
* visual mode is where you can make higlighted selection in the file 
**`v`** entering visual mode  
	* and then you can use it with any <motion_command>  
	<ins>Examples:</ins>
	`v$` select from cursor position until the end of the line
<motion command>

**`CTRL v`**  

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


