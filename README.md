# Extended Cursor Movements Extension

Written by Bill Stewart

This extension adds some additional cursor movement commands to VS Code:

* `extension.extendedCursorMove.cursorHome` - moves the cursor to the beginning of the current line, ignoring whitespace
* `extension.extendedCursorMove.cursorHomeSelect` - moves the cursor to the beginning of the current line, ignoring whitespace, and select
* `extension.extendedCursorMove.cursorHomeToNonWhitespace` - moves the cursor to the first non-whitespace character of the line
* `extension.extendedCursorMove.cursorEnd` - moves the cursor to the end of the current line after all whitespace
* `extension.extendedCursorMove.cursorEndSelect` - moves the cursor to the end of the current line after all whitespace and select
* `extension.extendedCursorMove.cursorTopLeft` - moves the cursor to the top left corner of the current view
* `extension.extendedCursorMove.cursorTopLeftSelect` - moves the cursor to the top left corner of the current view and select
* `extension.extendedCursorMove.cursorBottomRight` - moves the cursor to the bottom right corder of the current view
* `extension.extendedCursorMove.cursorBottomRightSelect` - moves the cursor to the bottom right corder of the current view and select
* `extension.extendedCursorMove.centerCursorInView` - moves the cursor to the center of the current view
* `extension.extendedCursorMove.moveCursorToView` - moves the cursor to the center of the current view

The `extension.extendedCursorMove.moveCursorToView` command can be useful if you have scrolled the cursor out of the current view and you want to position the cursor to the current view without using the mouse.

You can use these commands in your `keybindings.json` file; for example:

    [
      { "key": "home",       "command": "extension.extendedCursorMove.cursorHome",       "when": "editorTextFocus" },
      { "key": "end",        "command": "extension.extendedCursorMove.cursorEnd",        "when": "editorTextFocus" },
      { "key": "shift+home", "command": "extension.extendedCursorMove.cursorHomeSelect", "when": "editorTextFocus" },
      { "key": "shift+end",  "command": "extension.extendedCursorMove.cursorEndSelect",  "when": "editorTextFocus" }
    ]
