# VIM Editor Commands

## Modes

- **Normal Mode:** Press `Esc` to enter this mode (default mode for navigation and command execution).
- **Insert Mode:** Press `i`, `I`, `a`, `A`, `o`, or `O` to start inserting text.
- **Visual Mode:** Press `v` for character-wise selection, `V` for line-wise selection, or `Ctrl+v` for block selection.
- **Command Mode:** Press `:` to enter commands at the bottom line.

## Basic Commands

- `:q` - Quit VIM.
- `:q!` - Quit without saving changes.
- `:w` - Save the file.
- `:wq` or `:x` - Save and quit.
- `:e filename` - Open a file.
- `:sav filename` - Save the file under a new name.
- `:r filename` - Read contents of a file and insert them.
- `:w !sudo tee %` - Save a file with root permissions.

## Navigation

- `h` - Move left.
- `l` - Move right.
- `j` - Move down.
- `k` - Move up.
- `0` - Move to the beginning of the line.
- `^` - Move to the first non-whitespace character.
- `$` - Move to the end of the line.
- `gg` - Move to the beginning of the file.
- `G` - Move to the end of the file.
- `nG` - Go to the nth line.
- `Ctrl+d` - Scroll half a screen down.
- `Ctrl+u` - Scroll half a screen up.

## Editing

- `i` - Insert before the cursor.
- `I` - Insert at the beginning of the line.
- `a` - Append after the cursor.
- `A` - Append at the end of the line.
- `o` - Open a new line below.
- `O` - Open a new line above.
- `dd` - Delete the current line.
- `dw` - Delete the word from the cursor.
- `d$` - Delete from the cursor to the end of the line.
- `d0` - Delete from the cursor to the beginning of the line.
- `x` - Delete the character under the cursor.
- `u` - Undo the last change.
- `Ctrl+r` - Redo the undone change.
- `yy` - Yank (copy) the current line.
- `yw` - Yank the word from the cursor.
- `y$` - Yank to the end of the line.
- `p` - Paste after the cursor.
- `P` - Paste before the cursor.

## Search

- `/pattern` - Search for `pattern` forward.
- `?pattern` - Search for `pattern` backward.
- `n` - Repeat the search in the same direction.
- `N` - Repeat the search in the opposite direction.
- `:%s/old/new/g` - Replace all occurrences of `old` with `new` in the file.
- `:%s/old/new/gc` - Replace all occurrences with confirmation.

## Visual Mode Operations

- `v` - Start visual mode for character-wise selection.
- `V` - Start visual mode for line-wise selection.
- `Ctrl+v` - Start block selection.
- `d` - Delete the selected text.
- `y` - Yank the selected text.
- `>` - Indent the selection.
- `<` - Unindent the selection.

## Window Management

- `:sp filename` - Split the window horizontally and open a file.
- `:vsp filename` - Split the window vertically and open a file.
- `Ctrl+w` + `h` / `j` / `k` / `l` - Navigate between splits.
- `Ctrl+w` + `=` - Equalize split sizes.
- `Ctrl+w` + `q` - Close the current split.

## Registers

- `"ayy` - Yank a line into register `a`.
- `"ap` - Paste from register `a`.

## Macros

- `q<register>` - Start recording a macro in the specified register.
- `q` - Stop recording.
- `@<register>` - Execute the recorded macro.
- `@@` - Repeat the last macro.

## Tabs

- `:tabnew filename` - Open a file in a new tab.
- `gt` - Switch to the next tab.
- `gT` - Switch to the previous tab.
- `:tabclose` - Close the current tab.
- `:tabs` - List all open tabs.

## Buffers

- `:ls` - List all buffers.
- `:b <buffer_number>` - Switch to the specified buffer.
- `:bd` - Close the current buffer.

## Miscellaneous

- `:set number` - Show line numbers.
- `:set nonumber` - Hide line numbers.
- `:set hlsearch` - Highlight search results.
- `:set nohlsearch` - Remove search highlights.
- `:syntax on` - Enable syntax highlighting.
- `:syntax off` - Disable syntax highlighting.

