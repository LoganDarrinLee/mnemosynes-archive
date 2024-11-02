This is the second most used mode, and will be the most familiar behavior to most people. Once in insert mode, typing inserts characters just like a regular text editor. You can enter it by using an insert command from normal mode.

Insert commands include:

- `i` for insert, this immediately switches vim to insert mode
- `a` for **a**ppend, this moves the cursor after the current character and enters insert mode
- `o` inserts a new line below the current line and enters insert mode on the new line

These commands have an uppercase variety too:

- `I` moves the cursor to the beginning of the line and enters insert mode
- `A` moves the cursor to the end of the line and enters insert mode
- `O` inserts a new line above the current one and enters insert mode on the new line

There are so many more ways of inserting text in Vim that can’t be listed here but these are the simplest. Also, beware of staying in insert mode for too long; Vim is not designed to be used in insert mode all the time.

To leave insert mode and return to normal mode, press `Esc` or `<C-[>`