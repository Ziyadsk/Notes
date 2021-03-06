# VIM

Vim is a modal text editor, open-source and available in almost all operating systems, especially [Apple MacOS](https://en.wikipedia.org/wiki/MacOS) and also on almost every [linux](https://en.wikipedia.org/wiki/Linux) distribution out there and apple.

Vim is powerful, fast and efficient due to its ability to separates the idea of actions,moving and editing of a file.

Vim has more than 10 modes but these 4 are the most important :
- **Normal** mode
- **Insert** mode 
- **Visual** mode
- **Command-line** mode

> **Note** : By default when you enter vim you are in **NORMAL** mode
>$ -  if you enter any other mode to go back to the **NORMAL** mode press <kbd>ESC</kbd>


## Table of content
* [**NORMAL** Mode](#normal)
	* [Motions](#motions)
	* [Actions](#actions)
		* [Indentation](#indentation)
		* [Deletion](#deletion)
		* [Copy and paste](#copy)
		* [Replace](#replace)
		* [Undo and redo](#undo-and-redo)
		* [More Commands](#more)
* [**INSERT** Mode](#insert)
* [**VISUAL** Mode](#visual)
* [**COMMANDLINE** Mode](#commandLine)
* [**Tabs and split**](#tabs)
* [**The Vimrc**](#vimrc)
* [**VimScript**](#vimscript)

<a id='normal'></a>
## NORMAL MODE
## *Motions*
Moving in vim is done mainly in **NORMAL** mode.  

Here are the most used motions keybinding :   

**`0`** to go the start of the line  

**`^`** jump to first non-whitespace character on the line

**`$`** to go the end of the line  

**`%`** to jump between {} or [] or ()   

**`w`** and b jump by words forwards and backwards  

**`e`** to jump by words but puts cursor at the end of line  

**`{`** and **`}`** jump blocks forwards and backwards  

**`f<CHAR>`** jump to the first `<CHAR>` in that line 

**`t<CHAR>`** jump one character before the first <CHAR> in that line   

**`gg`** to jump to head of the file

**`G`** to jump to end of the file

**`gd`** to jump to definition

**`df`** go the file under the cursor 

### using count with motions
- vim support giving count to motions or actions
	* <ins>Examples:</ins>  
	**`3j`** moves 3 lines down  
	**`10w`** moves 10 words forwards

<a id='action'></a>

## *Actions*
<a id="indentation"></a>

### Indentation
**`>>`** indent  
**`<<`** dedent  
**`>%`** indent a block  
**`<%`** dedent a block  

<a id='deletion'></a>

### Deletion
**`x`** deletes the character under the cursor  
**`daw`** deletes the word under the cursor  
**`dip`** deletes a paragraph  
**`dap`** deletes a paragraph and the whitespace surrounding it  
**`d`** <motion_command>  

<ins>Examples:</ins>  

**`dw`** deletes until the end of the word under the cursor  
**`dd`** deletes the entire line  
**`d$`** deletes from cursor position to the end of the line  
**`d0`** deletes from cursor position to the start of the line  
**`dgg`** deletes from cursor position to the start of the line  
**`dG`** deletes from cursor position to the end of the line  
**`db`** deletes a words from cursor position  
**`df<CHAR>`** deletes from cursor until character `<CHAR>`  
>works also with counts  

**`d3w`** **d**eletes **3** **w**ords   
**`3dd`** deletes 3 lines	

> deletion also act as copying so when you **`dd`** a line you can just paste it with **`p`**  

<a id='copy'></a>

### Copy and paste
**`yy`** copies the entire line  
**`p`** paste  
**`y`** <[motion_command](#motions)>  
* <ins>Examples</ins>:   
	**`y$`** copies from the cursor position to the end of the line  
	**`yG`** copies from the cursor position to the end of the file  
	**`ygg`** copies from the cursor position to the beginning of the file  
	**`yw`** copies from the cursor position until the end of the word under the cursor  
	**`yaw`** copies the entire word under the cursor  
	>  works also with counts 

	**`10yy`** copy 10 lines from where the cursor is

<a id='replace'></a>

### Replace

**`r<CHAR>`** to replace the word under the cursor with a character `<CHAR>`   
**`cc`** deletes line and puts you in insert mode    
**`c`** <[motion_command](#motions)> 
* <ins>Examples:</ins>   
	**`cw`** delete word and puts you in insert mode  
	**`c$`** deletes from cursor position to the end of the line and puts you in insert mode  
	**`c0`** deletes from cursor position to the start of the line and puts you in insert mode  
	**`cgg`** deletes from cursor position to the start of the line and puts you in insert mode  
	**`cG`** deletes from cursor position to the end of the line and puts you in insert mode  
	**`cb`** deletes a words from cursor position and puts you in insert mode   
	**`cf<CHAR>`** deletes to the first occureence of `<CHAR>` and puts you in insert mode  
	
	>  works also with counts  

	**`3cc`** deletes 3 lines and enters insert mode

**`R`** enters replace mode (you can keep replacing until quitting with <button>ESC</button>)  

<a id='undro'></a>

### Undo and redo
**`u`** to undo the last action  
**`CTRL+r`** to redo  
**`.`** is used to repeat the last action  

<a id='more'></a>

### More
**`K`** opens manpage for the command under the cursor  
**`J`** joins below with the current one

**`gU`** change to upperCase the current character   
**`gu`** change to lowercase the current character  
**`g~`** toggle the case of the current character  
**`gUaw`** to change a **w**ord to **U**ppercase

**`CTRL a`** increments a number     

<a id='insert'></a>

## INSERT MODE
* insert mode is where you change text inside the file you opened

**`i`** enter insert mode under the cursor    
**`a`** move one character forwards and start insert mode    
**`I`** enter insert mode at the start of the line  
**`A`** enter insert mode at the end of the line  
**`o`** creates a new line under the cursor line and then enters insert mode  
**`O`** creates a new line above  the cursor line and then enters insert mode

<a id='visual'></a>

## VISUAL MODE
* **VISUAL** mode is where you can make higlighted selection in the file 
**`v`** entering visual mode  
	* and then you can use it with any <[motion_command](#motions)> to select and then you can preform any <[action_command](#actions)> on the selection  
	<ins>Examples:</ins>  
	**`v$`** select from cursor position until the end of the line  
	**`vgg`** select from cursor until the start of the file    
	**`vfk`** select until the first occcurrence of k starting from where the cursor is  
	**`v4w`** select until the 4 words from where the cursor is   
	**`v10kU`** change the 10 lines above into uppercase  

	> special commands   
	
	**`vab`** to select everything between a pair of parentheses  
	**`vaB`** to select everything between a pair of curly braces  
	**`vat`** to select everything between a pair of `<>`  
> O is used to move between the ends and the beginning of the selection

* **`CTRL v`** enters visual-block (**V-BLOCK**) mode

	* **V-BLOCK** mode is like visual mode but the selection is done on columns   
		* <ins>Example</ins>:  
	**`CTRL v 4kI #<ESC>`** prefixes the 4 lines above with the `#` symbol.


>  Note : selecting in **VISUAL** mode and then going the to *COMMANDLINE MODE* is very powerful :    

<ins>Example</ins>:  

**`norm <ANY_EX_COMMAND>`** execute an ex command on all the the selected lines

<a href="commandLine"></a>

## Command-line mode or EX commands
You enter an Ex command by pressing **`:`** from **NORMAL** mode
* Your command are written after the `:` that will appears at the bottom of the screen and when you are done writing the command press **<input type=submit value=ENTER>** to execute that command and you will be back in **NORMAL** mode. 

**`<NUMBER>`** goes to that line
* <ins>Examples:</ins>  
	`:142` goes to the line number 142

**`w`** to save the current file  
**`e <FILENAME>`** opens the `<FILENAME>` in vim  
**`q`** quits vim  
**`earlier <NUMBER><m/h/s>`** Go back to the state of the file by specifing the time   
- <ins>Example:</ins>  
	`:earlier 10s`  
	`:earlier 1h`

**`later <NUMBER><m/h/s>`** Go back to the state of the file by specifing the time 
- <ins>Example:</ins>  
	`:later 30s`  
	`:later 52m`

**`%s/<REPLACED_TEXT>/<WHAT_TO_REPLACE_WITH>/<FLAG>`**  
* <ins>Examples</ins>:  
	**`:%s/james/donald/g`** replace all occurrences of james with donald in the file

**`/`** search for a pattern (doesn't need to be prefixed with `:`)
- <ins>Examples:</ins> 
	`/John` matches all the 'john' in the file  
	`/^k` matches every lines that begins with `k`  
	`/y$` matches every lines that ends with `y`  
	- when multiple matches are found:  
		**`n`** to go to the next occurrence  
		**`N`** to go the previous occurrence	

**`!<EXTERNAL_COMMAND>`** run an external command  
- <ins>Examples</ins>:  
		**`:!ls`**  
		**`:!touch newFile`**

**`:help <WORD>`** displays the help for any command in vim

<a id='tabs'></a>

## Tabs and Splits
`@TODO`

<a id='vimrc'></a>

## The .vimrc (Vim's configuration file)
The `.vimrc` is vim's configuration file.  

`@TODO`

<a id='vimscript'></a>

## Vimscript
`@TODO`


## Encrypting a file using vim
`:X`