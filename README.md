# ydo - a ydotool wrapper

This script is a simple wrapper around [ydotool](https://github.com/ReimuNotMoe/ydotool) that uses key mnemonics instead of the hex codes.

**ydo** tries to parse the mnemonics from **/usr/include/linux/input-event-codes.h** if available on the system, if not it uses built-in mappings.

Usage examples:

```bash
# Type text
./ydo type "Hello world!"

# Press Enter key
./ydo key KEY_ENTER:1 KEY_ENTER:0

# Type with custom delay
./ydo type -d 20 "Slow typing"

# Type from file
./ydo type -f input.txt
```
