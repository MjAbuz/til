# Format Long Lines To Text Width

Vim allows you to set the maximum width for text per line in a buffer. For
example, you can set the maximum text width to 80 characters like so:

```
:set textwidth=80
```

With this set, vim will automatically break on whitespace whenever you hit
80 characters. There are two places where this doesn't quite pan out. You
will see this as soon as you open a file with lines of text that exceed 80
characters and when you paste long lines of text into your buffer. You can
quickly remedy this with `gw`.

Make a visual selection of the lines that need formatting and then hit `gw`.
All the lines should then we truncated to 80 or less characters.