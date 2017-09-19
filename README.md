# VIM
### Commandline
`vim filename` Opens new file in Vim
`vim -N` opens Vim in new mode incopatible with Vi

### General
 `ctrl + L` refreshes screen
 `:w !sudo tee %` saves the file with sudo
## Settings
### option tricks
* `:set list` or `set nolist` - turn on/off
* `:set list?` show current value
* `:set list&` set to default value 
### set
* `:set ruler` show the cursor position in the status bar
* `:set number` show line numbers
* `:set laststatus` always show the statusbar
* `:set syntax=enable` enable syntax highlighting
* `:set filetype=xml` sets syntax to XML
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
* `:set softtabstop=2` control how many columns vim uses when you hit Tab in insert mode
* `:`

## Visual mode
* `o` in selection toggles cursor between first and last cursor positions

