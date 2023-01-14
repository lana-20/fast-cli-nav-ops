# A fast way to navigate over command line in a shell program.

Bash, a common shell, uses the Readline library to implement command line input and navigation.


| Command | Description | Command Type |
--- | --- | --- |
|<kbd>Ctrl</kbd>+<kbd>B</kbd>|Move back one character.|Essentials|
|<kbd>Ctrl</kbd>+<kbd>F</kbd>|Move forward one character.|Essentials|
|<kbd>Ctrl</kbd>+<kbd>D</kbd>|Delete the character underneath the cursor.|Essentials|
| <kbd>⌫ Delete</kbd> or <kbd>⌫ Backspace</kbd>|Delete the character to the left of the cursor.|Essentials|
|<kbd>Ctrl</kbd>+<kbd>_</kbd>, <kbd>Ctrl</kbd>+<kbd>X</kbd>, <kbd>Ctrl</kbd>+<kbd>U</kbd>, or <kbd>Ctrl</kbd>+<kbd>/</kbd>|Undo the last editing command. You can undo all the way back to an empty line.|Essentials|
|<kbd>Ctrl</kbd>+<kbd>A</kbd>|Move to the start of the line.|Movement|
|<kbd>Ctrl</kbd>+<kbd>E</kbd>|Move to the end of the line.|Movement|
|<kbd>⎇ Meta</kbd>+<kbd>F</kbd> or <kbd>⎇ Alt</kbd>+<kbd>F</kbd> or <kbd>⎇ Option</kbd>+<kbd>F</kbd>|Move forward a word, where a word is composed of letters and digits.|Movement|
|<kbd>Ctrl</kbd>+<kbd>L</kbd>|Clear the screen, reprinting the current line at the top.|Movement|



Readline can operate in two modes:

- emacs mode (default)
- _vi mode_

Switch Bash to use vi mode by typing:

    $ set -o vi

In macOS Terminal app (and in [iTerm](https://iterm2.com/) emulator), perform <kbd>Option</kbd>+Click to move the cursor. The cursor will move to the clicked position. This also works inside _vim_.

----
🔗

[Bash (Unix shell)](https://en.wikipedia.org/wiki/Bash_%28Unix_shell%29)

[GNU Readline](https://en.wikipedia.org/wiki/GNU_Readline)

[GNU Readline Library](https://tiswww.case.edu/php/chet/readline/readline.html#SEC22)

[GNU Readline Documentation](https://www.gnu.org/software/bash/manual/bash.html#Readline-Interaction)

[vi Editor Cheat Sheet](https://github.com/lana-20/fast-cli-nav/blob/main/vi_cheat_sheet.pdf)
