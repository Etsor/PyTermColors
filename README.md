Simple Python class with ANSI escape codes for styling and coloring terminal output

---

## Installation

Just copy `pytermcolors.py` into your project folder

---

## Usage

```python
from pytermcolors import PyTermColors

style = PyTermColors

print(f"{style.BOLD}{style.FG_GREEN}Ok!{style.RESET}")
print(f"{style.UNDERLINE}{style.FG_YELLOW}Warning!{style.RESET}")
print(f"{style.FG_RED}{style.BG_BRIGHT_WHITE}{style.STRIKETHROUGH}Error!{style.RESET}")
```

Or:

```python
from pytermcolors import colorize, PyTermColors as s

print(colorize("Hello World!", fg=s.FG_CYAN, bg=s.BG_BLACK, bold=True, italic=True))
print(colorize("Warning!", fg=s.FG_YELLOW, bold=True, underline=True))
print(colorize("Error!", fg=s.FG_RED, strike=True))
```

![example](res/example.png)
