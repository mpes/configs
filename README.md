# VIM
### Commandline
`vim filename` Opens new file in Vim
`vim -N` opens Vim in new mode incopatible with Vi

### Keyboard shortcuts

* <kbd>ctrl + L</kbd> refreshes screen
* <kbd>ctrl + ^</kbd> switches to next file when multiple opened
* 
### General 
 `:w !sudo tee %` saves the file with sudo
 <kbd>ctrl + r =</kbd> you can type expressions *2+2* or system commands *system('pwd')* and results will be placed at cursor when in insert mode
 
## Settings
### marks
* `ma` creates mark named *a*
* `` `a`` jumps to mark *a* position
* `'a` jumps to the begginning of the line of mark *a*
### options tricks

* `:set list` or `:set nolist` - turn on/off
* `:set list?` show current value
* `:set list&` set to default value  

### set operation

* `:set list` show hidden characters
* `:set ruler` show the cursor position in the status bar
* `:set number` show line numbers
* `:set laststatus` always show the statusbar
* `:set syntax=enable` enable syntax highlighting
* `:set filetype=xml` sets syntax to XML
* `:set softtabstop=2` control how many columns vim uses when you hit Tab in insert mode
* `:e .` browse directory
 `i` long, wide or tree
 `s` sort on name, siize or date
 `r` reverse order
 `gh` hide/show dotfiles
 `x` opens with associated application
 `d` makes directory
 `D` deletes file or dir
 `R` renames
 `-` goes up one level
* `:e filename` opens a file
* `:cd path` changes working directory. Then we can use relative paths and use TAB to autocomplete
### search and replace
|Range|Description|Example|
|-------|-----------|---------|
|21|line 21|21s/old/new/g|
|1|first line|1s/old/new/g|
|$|last line|$s/old/new/g|
|.|current line|.w single.txt|
|%|all lines (same as 1,$)|%s/old/new/g|
|21,25|lines 21 to 25 inclusive|21,25s/old/new/g|
|21,$|lines 21 to end|21,$s/old/new/g|
|.,$|current line to end|.,$s/old/new/g|
|.+1,$|line after current line to end|.+1,$s/old/new/g|
|.,.+5|six lines (current to current+5 inclusive)|.,.+5s/old/new/g|
|.,.5|same (.5 is interpreted as .+5)|.,.5s/old/new/g|

### delete
* `:1,.d` deletes from first line to current(included)
* `:.+1,$-1d` deletes from first line to current (included)

## Visual mode
* `o` in selection toggles cursor between first and last cursor positions

## Insert mode
* `ctrl+d` shift text left in insert mode
* `ctrl+t` shift text right in insert mode

###Tips
* `:123put =range(11,15)`  inserts number 11-15 after line number 123
* `:for i in range(1,10) | put ='192.168.0.'.i | endfor` generates ip addresses 192.168.0.1 to 192.168.0.10

