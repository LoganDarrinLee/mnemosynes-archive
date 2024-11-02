Visual mode is used to make selections of text, similar to how clicking and dragging with a mouse behaves. Selecting text allows commands to apply only to the selection, such as copying, deleting, replacing, and so on.

To make a text selection:

- Press `v` to enter visual mode, this will also mark a starting selection point
- Move the cursor to the desired end selection point; vim will provide a visual highlight of the text selection

Visual mode also has the following variants:

- `V` to enter visual line mode, this will make text selections by line
- `<C-V>` to enter visual block mode, this will make text selections by blocks; moving the cursor will make rectangle selections of the text

To leave visual mode and return to normal mode, press `Esc` or `<C-[>`.

The visual mode actually has multiple subtypes: _visual_, _block-visual_ and _linewise-visual_

- _visual_: like described above. Enter by pressing `v`
- _block-visual_: select any rectangular region. Enter by pressing `<ctrl>+v`
- _linewise-visual_: always select full lines. Enter by pressing `<shift>+v`