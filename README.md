# Typewriting Effect Template

Hi folks! Today I'll be introducing a template that creates a cool typewriting effect that'll be perfect for console-based games in Python.

## Guide

To get started, open `main.py`. We already have the libaries needed (`os`, `time` and `sys`), and now we'll go over the code.

On line 5, we have the `write()` function.

```py
def write(text, speed=0.04):
  for char in text:
    sys.stdout.write(char)
    sys.stdout.flush()

    time.sleep(speed)

  print("")
  ```

We have two parameters, `text` and `speed`. The first parameter, `text`, is just the text you want to typewrite. The second parameter, `speed` is set to 0.04 seconds by default and will stay like that unless you change it.

On the next line, we use a `for` loop to get every character one-by-one from the text. We use `sys.stdout.write(char)` to write the character, and `sys.stdout.flush()` to flush the current text displayed. We then delay the code by using `time.sleep(sleep)` to pause the program to whatever speed you set it to. That means, the text will be more fastly displayed if `speed` is smaller, and will take a little longer to display if `speed` is bigger.

On the last line, we use `print("")` to parse a new line, so that we don't need to use `\n` for the end of everything. However, feel free to remove this, as its unnecessary for single-line parses, which you probably don't need for your console-based game.

Well, there you have it folks! That's all for today, and stay tuned for more projects and templates like this!