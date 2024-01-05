# Base 16 template for Ghostty

You can use l0go's site at https://l0go.github.io/ghostty-base16-converter/ to generate the theme directly in your web browser, without installing anything.

Of if you want to generate the color config manually, first install Mustache.

Then run:

```sh
mustache base16.mustache
```

Then paste in a theme you copied from
https://github.com/tinted-theming/base16-schemes
into the stdin, then press CTRL-D.

Your theme will be printed to stdout.

Here is an automatic script that does this all if you're on Wayland on Linux:

```sh
wl-paste | mustache base16.mustache >> ~/.config/ghostty/config
```

Note that if you are on NixOS, I've created a flake that handles it all:
https://github.com/RGBCube/ThemeNix.

## License

```
MIT License

Copyright (c) 2023-present RGBCube

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
