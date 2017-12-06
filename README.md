# hsa_ufa
This is a re-implementation of the old hsa console by Holt Software Associates.
Re-done from scratch in Swing with much code imported from the old hsa console.
The main goals were to reduce screen flicker during animations and eliminate a 
couple of small bugs in the input routines. April 30, 2010.
  
Differences from hsa console:
  - Row & Column for text start at 0, 0
  - When creating console, specify width, height in pixels (not rows, columns)
  - setColor sets the drawing color for print and println as well as graphics
  - setTextBackgroundColor no longer works. Use setBackgroundColor instead.
  - use getDrawHeight() and getDrawWidth() for screen size in pixels
  - no more readString. Use readToken or readLine instead.
  - no more readChar. Use getChar instead.
  - methods added to poll the keyboard state without pausing the program (ketKeyChar, 
    getKeyCode, getLastKeyChar, etc.). Good for live-action games.
  - dropped support for print, quit, save buttons.
  - fixed drawImage to be more reliable
  
Author: Sam Scott / Tom West (old hsa code)
