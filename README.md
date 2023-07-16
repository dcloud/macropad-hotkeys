# macropad-hotkeys

Adapting the [Adafruit MacroPad Hotkeys](https://learn.adafruit.com/macropad-hotkeys/project-code) project.

The project depends on the `lib` folder containing Adafruit CircuitPythong libraries downloaded from the [Project Bundle](https://learn.adafruit.com/pages/22617/elements/3099360/download?type=zip).

## Installation

In the past, I've written Makefiles to automate downloading libraries and installing things. IDK if I want to do that again, but the bit below will copy files without extended attributes (the `-X` option for cp).


```
board="/Volumes/CIRCUITPY"
cp -rXv lib "$board"
cp -rXv macros "$board"
cp -Xv code.py "$board"
```

## References/Inspiration
- [CircuitPython MacroPad board page](https://circuitpython.org/board/adafruit_macropad_rp2040/)
- [Awesome MacroPad](https://github.com/prcutler/awesome-macropad)

