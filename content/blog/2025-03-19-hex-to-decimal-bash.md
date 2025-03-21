---
title: Convert Hex to Decimal in Bash
description: One approach to convert a Hex value to Decimal
date: 2025-03-19
tags: [Hex, Bash]
---

For reasons I don't fully recall—probably because I was searching for colors to style my web site—I found myself frequently converting hex values to decimal. I quickly grew tired of searching online for a hex converter every time, so I wondered if there was a simpler way to do it directly in the terminal.

Turns out, there is! You can use a simple one-liner in Bash:

```bash
$ echo $(( 16#FF ))
255
```

Neat, simple, and no need to repeat the same search online!

---

### But how does it work?

Bash provides several ways to perform arithmetic operations, but for integer calculations, the recommended approach is to use its built-in [Arithmetic Expansion](https://www.gnu.org/software/bash/manual/html_node/Arithmetic-Expansion.html) feature. This allows you to evaluate expressions within double parentheses:

```bash
$(( expression ))
```

For example:

```bash
$ echo $(( 40 + 2 ))
```

By default, Bash arithmetic works in base 10. However, you can specify a different base using the syntax *base#number*. Regardless of the original base, arithmetic expansion always returns the decimal equivalent. This makes it easy to convert hexadecimal values:

```bash
$ echo $(( 16#2A ))
42
```

This method is useful for quick conversions, but be cautious when using it for validation. For example:

```bash
$ HEX='F+!P4_'
$ echo $(( 16#$HEX ))
16
```

This result is misleading because *F+!P4_* is not a valid hexadecimal number. Thus, I wouldn’t rely on this method in a script if input validation is required.

An alternative approach is to use `printf`:

```bash
$ printf "%d\n" 0x0F
15
```

However, it has similar issues:

```bash
$ HEX='F+!P4_'
$ printf "%d\n" 0x$HEX
16
```

So while these methods are handy for quick conversions, they shouldn't be trusted for strict hex validation. Use them wisely!
