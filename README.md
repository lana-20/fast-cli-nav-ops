# A fast way to navigate over command line in a shell program.

Bash, a common shell, uses the Readline library to implement command line input and navigation.


| Command | Description | Command Type |
--- | --- | --- |
|<kbd>Ctrl</kbd>+<kbd>B</kbd>|Move back one character.|Essentials|
|<kbd>Ctrl</kbd>+<kbd>F</kbd>|Move forward one character.|Essentials|
|<kbd>Ctrl</kbd>+<kbd>D</kbd>|Delete the character underneath the cursor.|Essentials|
|<kbd>⌫ Delete</kbd> or <kbd>⌫ Backspace</kbd>|Delete the character to the left of the cursor.|Essentials|
|<kbd>Ctrl</kbd>+<kbd>_</kbd>, <kbd>Ctrl</kbd>+<kbd>X</kbd>, <kbd>Ctrl</kbd>+<kbd>U</kbd>, or <kbd>Ctrl</kbd>+<kbd>/</kbd>|Undo the last editing command. You can undo all the way back to an empty line.|Essentials|
|<kbd>Ctrl</kbd>+<kbd>A</kbd>|Move to the start of the line.|Movement|
|<kbd>Ctrl</kbd>+<kbd>E</kbd>|Move to the end of the line.|Movement|
|<kbd>⎇ Meta</kbd>+<kbd>F</kbd>, <kbd>⎇ Alt</kbd>+<kbd>Shift</kbd>+<kbd>F</kbd> or <kbd>⎇ Option</kbd>+<kbd>Shift</kbd>+<kbd>F</kbd>|Move forward a word, where a word is composed of letters and digits.|Movement|
|<kbd>⎇ Meta</kbd>+<kbd>B</kbd>, <kbd>⎇ Alt</kbd>+<kbd>Shift</kbd>+<kbd>B</kbd> or <kbd>⎇ Option</kbd>+<kbd>Shift</kbd>+<kbd>B</kbd>|Move backward a word.|Movement|
|<kbd>Ctrl</kbd>+<kbd>L</kbd>|Clear the screen, reprinting the current line at the top.|Movement|
|<kbd>Ctrl</kbd>+<kbd>K</kbd>|Kill the text from the current cursor position to the end of the line.|Kill & Yank (aka Cut & Paste)|
|<kbd>⎇ Meta</kbd>+<kbd>D</kbd>, <kbd>⎇ Alt</kbd>+<kbd>Shift</kbd>+<kbd>D</kbd>, or <kbd>⎇ Option</kbd>+<kbd>Shift</kbd>+<kbd>D</kbd>|Kill from the cursor to the end of the current word, or, if between words, to the end of the next word. Word boundaries are the same as those used by <kbd>⎇ Meta</kbd>+<kbd>F</kbd>.|Kill & Yank (aka Cut & Paste)|
|<kbd>⎇ Meta</kbd>+<kbd>⌫ Delete</kbd>, <kbd>⎇ Alt</kbd>+<kbd>Shift</kbd>+<kbd>⌫ Delete</kbd>, or <kbd>⎇ Option</kbd>+<kbd>Shift</kbd>+<kbd>⌫ Delete</kbd>|Kill from the cursor to the start of the current word, or, if between words, to the start of the previous word. Word boundaries are the same as those used by <kbd>⎇ Meta</kbd>+<kbd>B</kbd>.|Kill & Yank (aka Cut & Paste)|
|<kbd>Ctrl</kbd>+<kbd>W</kbd>|Kill from the cursor to the previous whitespace. This is different from <kbd>⎇ Meta</kbd>+<kbd>⌫ Delete</kbd>, because the word boundaries differ.|Kill & Yank (aka Cut & Paste)|
|<kbd>Ctrl</kbd>+<kbd>Y</kbd>|Yank the most recently killed text back into the buffer at the cursor.|Kill & Yank (aka Cut & Paste)|
|<kbd>⎇ Meta</kbd>+<kbd>Y</kbd>, <kbd>⎇ Alt</kbd>+<kbd>Shift</kbd>+<kbd>Y</kbd>, or <kbd>⎇ Option</kbd>+<kbd>Shift</kbd>+<kbd>Y</kbd>|Rotate the kill-ring, and yank the new top. You can only do this if the prior command is <kbd>Ctrl</kbd>+<kbd>Y</kbd> or <kbd>⎇ Meta</kbd>+<kbd>Y</kbd>.|Kill & Yank (aka Cut & Paste)|

Readline can operate in two modes:

- emacs mode (default)
- _vi mode_

Switch Bash to use vi mode by typing:

    $ set -o vi

In macOS Terminal app (and in [iTerm](https://iterm2.com/) emulator), perform <kbd>Option</kbd>+Click to move the cursor. The cursor will move to the clicked position. This also works inside _vim_.

For Max OS X Terminal, you can enable "Use option as meta key" in Settings/Keyboard.
For iTerm, the <kbd>⎇ Meta</kbd> key doesn't work, until the following setting is configured __Preferences > Profiles > Default > Keys > Left/Right option key acts as +Esc__. 
For Linux, in the standard Ubuntu terminal, for example,  <kbd>⎇ Meta</kbd> is <kbd>⎇ Alt</kbd>+<kbd>Shift</kbd>, unless you disable the menu access keyboard shortcuts in which case it is just <kbd>⎇ Alt</kbd>. 

----
🔗

[Bash (Unix shell)](https://en.wikipedia.org/wiki/Bash_%28Unix_shell%29)

[GNU Readline](https://en.wikipedia.org/wiki/GNU_Readline)

[GNU Readline Library](https://tiswww.case.edu/php/chet/readline/readline.html#SEC22)

[GNU Readline Documentation](https://www.gnu.org/software/bash/manual/bash.html#Readline-Interaction)

[vi Editor Cheat Sheet](https://github.com/lana-20/fast-cli-nav/blob/main/vi_cheat_sheet.pdf)

[Stackoverflow Discussion](https://stackoverflow.com/questions/657130/fastest-ways-to-move-the-cursor-on-a-terminal-command-line)
