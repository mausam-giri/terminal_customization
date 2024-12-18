# Terminal Customization
## Color to Text in Python

To make some of text more readable,  use [ANSI escape codes](https://en.wikipedia.org/wiki/ANSI_escape_code) to change the colour of the text output in the python program. A good use case for this is to highlight errors.
##### The escape codes are entered right into the print statement.
``` python 
print("\033[1;32;40m Bright Green \n")
```

##### The above ANSI escape code will set the text colour to bright green. The format is;
``` 
\033[ Escape code, this is always the same
1 = Style, 1 for normal.
32 = Text colour, 32 for bright green.
40m = Background colour, 40 is for black.
```

This table shows some of the available formats;
| TEXT COLOR | CODE | TEXT STYLE | CODE | BACKGROUND COLOR | CODE |
|--|--|--|--|--|--|
| Black | 30 | No Effect | 0 | Black | 40 |
| Red | 31 | Bold | 1 | Red | 41 |
| Green | 32 | Underline | 2 | Green | 42 |
| Yellow | 33 | Negative | 3 | Yellow | 43 |
| Blue | 34 | Negative 2 | 5 | Blue | 44 |
| Purple | 35 |  |  | Purple | 45 |
| Cyan | 36 |  |  | Cyan | 46 |
| White | 37 |  |  | White | 47 |

##### Here is the code used to create the coloured text.
``` python
print("\033[0;37;40m Normal text\n")
print("\033[2;37;40m Underlined text\033[0;37;40m \n")
print("\033[1;37;40m Bright Colour\033[0;37;40m \n")
print("\033[3;37;40m Negative Colour\033[0;37;40m \n")
print("\033[5;37;40m Negative Colour\033[0;37;40m\n")
print("\033[1;37;40m \033[2;37:40m TextColour BlackBackground TextColour GreyBackground WhiteText ColouredBackground\033[0;37;40m\n")
print("\033[1;30;40m Dark Gray \033[0m 1;30;40m \033[0;30;47m Black \033[0m 0;30;47m \033[0;37;41m Black \033[0m 0;37;41m")
print("\033[1;31;40m Bright Red \033[0m 1;31;40m \033[0;31;47m Red \033[0m 0;31;47m \033[0;37;42m Black \033[0m 0;37;42m")
print("\033[1;32;40m Bright Green \033[0m 1;32;40m \033[0;32;47m Green \033[0m 0;32;47m \033[0;37;43m Black \033[0m 0;37;43m")
print("\033[1;33;40m Yellow \033[0m 1;33;40m \033[0;33;47m Brown \033[0m 0;33;47m \033[0;37;44m Black \033[0m 0;37;44m")
print("\033[1;34;40m Bright Blue \033[0m 1;34;40m \033[0;34;47m Blue \033[0m 0;34;47m \033[0;37;45m Black \033[0m 0;37;45m")
print("\033[1;35;40m Bright Magenta \033[0m 1;35;40m \033[0;35;47m Magenta \033[0m 0;35;47m \033[0;37;46m Black \033[0m 0;37;46m")
print("\033[1;36;40m Bright Cyan \033[0m 1;36;40m \033[0;36;47m Cyan \033[0m 0;36;47m \033[0;37;47m Black \033[0m 0;37;47m")
print("\033[1;37;40m White \033[0m 1;37;40m \033[0;37;40m Light Grey \033[0m 0;37;40m \033[0;37;48m Black \033[0m 0;37;48m")
```
