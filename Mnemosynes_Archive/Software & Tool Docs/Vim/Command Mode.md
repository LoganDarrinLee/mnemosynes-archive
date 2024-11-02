
Command mode has a wide variety of commands and can do things that normal mode can’t do as easily. To enter command mode type ’:’ from normal mode and then type your command which should appear at the bottom of the window. For example, to do a global find and replace type `:%s/foo/bar/g` to replace all ‘foo’ with ‘bar’

- `:` Enters command mode
- `%` Means across all lines
- `s` Means substitute
- `/foo` is regex to find things to replace
- `/bar/` is regex to replace things with
- `/g` means global, otherwise it would only execute once per line

Vim has a number of other methods that you can read about in the help documentation, `:h` or `:help`.

## Commands
- `:%s/this/that/gc` Replace this with that, `/gc` is global to buffer. [More info](https://blog.beezwax.net/advanced-search-and-replace-with-vim/)