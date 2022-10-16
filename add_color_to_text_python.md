# Color to Text in Python

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
