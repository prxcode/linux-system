# Getting Started with Vim

### Opening Vim

```bash
vim <filename>     # Open file; creates it if it doesn't exist
```

---

## Basic Navigation (Normal Mode)

- `h`         : Move left
- `l`         : Move right
- `j`         : Move down
- `k`         : Move up
- `0`         : Move to beginning of line
- `^`         : Move to first non-blank character
- `$`         : Move to end of line
- `gg`        : Go to start of file
- `G`         : Go to end of file
- `:n`        : Go to line number `n`
- `Ctrl + d`  : Scroll half-page down
- `Ctrl + u`  : Scroll half-page up
- `Ctrl + f`  : Page down
- `Ctrl + b`  : Page up
- `zz`        : Center current line in window

---

## Editing Text (Insert & Normal Mode)

- `i`         : Insert before cursor
- `I`         : Insert at start of line
- `a`         : Append after cursor
- `A`         : Append at end of line
- `o`         : Open new line below
- `O`         : Open new line above
- `r<char>`   : Replace one character
- `R`         : Enter replace mode
- `x`         : Delete character under cursor
- `u`         : Undo
- `Ctrl + r`  : Redo
- `dd`        : Delete (cut) line
- `yy`        : Copy (yank) line
- `p`         : Paste after cursor
- `P`         : Paste before cursor
- `:w`        : Save file
- `:q`        : Quit Vim
- `:wq`       : Save and quit
- `:q!`       : Quit without saving

---

## Search & Replace

- `/pattern`          : Search forward
- `?pattern`          : Search backward
- `n`                 : Repeat last search forward
- `N`                 : Repeat last search backward
- `:%s/old/new/g`     : Replace all in file
- `:s/old/new/`       : Replace on current line
- `:%s/old/new/gc`    : Confirm each replace

---

## Working with Files

- `:e filename`   : Open another file
- `:w`            : Save current file
- `:w newfile`    : Save to a new file
- `:q`            : Quit
- `:q!`           : Quit without saving
- `:wq` or `ZZ`   : Save and quit

---

## Visual Mode (Selecting Text)

- `v`             : Start visual mode (character-wise)
- `V`             : Start line-wise visual mode
- `Ctrl + v`      : Start block (column) selection
- `y`             : Yank (copy) selection
- `d`             : Delete selection
- `p`             : Paste after selection

---

## Advanced Editing

- `%`             : Jump to matching bracket/brace
- `>>` / `<<`     : Indent/unindent line
- `=`             : Auto-indent code block
- `:set number`   : Show line numbers
- `:set relativenumber` : Show relative numbers
- `:set paste`    : Prevent auto-indent when pasting
- `:set nowrap`   : Disable line wrapping

---

## Example usage in Vim

1. Open a file:

   ```bash
   vim myfile.txt
   ```

2. Enter insert mode:

   - Press `i`

3. Write your content, then press `Esc` to return to normal mode.

4. Save and quit:

   - Type `:wq` then press `Enter`

