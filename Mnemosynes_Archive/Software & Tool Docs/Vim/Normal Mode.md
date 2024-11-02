By default, Vim starts in “normal” mode. Normal mode can be accessed from other modes by pressing `Esc` or `<C-[>`.

In Normal mode key presses don’t work as one would expect. That is, they don’t insert text into the document; instead, certain key presses can:

#### **Move the cursor**

- **h** move one character left
- **j** move one row down
- **k** move one row up
- **l** move one character right

As many vim commands, row movement can be prefixed by a number to move s everal lines at a time:

- **4j** move 4 rows down
- **6k** move 6 rows up

Basic word movements:

- **w** move to beginning of next word
- **b** move to previous beginning of word
- **e** move to end of word
- **W** move to beginning of next word after a whitespace
- **B** move to beginning of previous word before a whitespace
- **E** move to end of word before a whitespace

Beginning/End of line movement:

- **0** move to the beginning of the line
- **$** move to the end of the line

#### **Manipulate text**

#### **Enter other modes**

**Normal mode** is where one should spend most of their time while using Vim. Remember, this is what makes Vim different.

In normal mode, there are multiple ways to move around an open file. In addition to using the cursor keys to move around, you can use `h` (left), `j` (down), `k` (up), and `l` (right) to move as well. This particularly helps touch typists who don’t like leaving the home row when making changes.

You can also make changes to single characters in normal mode. For example, to replace a single character, move your cursor over it and press `r`, and then the character you want to replace it with. Similarly, you can delete single characters by moving your cursor over it and pressing `x`.

To perform an undo, press `u` in normal mode. This undoes changes up to the last time you were in normal mode. If you want to redo (_i.e._, undo your undo) press `Ctrl+r` in normal mode.