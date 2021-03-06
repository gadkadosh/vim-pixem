# Pix'em
This is my first vim plugin. Not terribly useful but a good way to learn some basic Vimscript.
## What it does
Converts between px and em values, for example in css stylesheets.
## How to install it
If you use vim-plug simply drop this line into your vimrc, or do the equivalent thing for your plugin manager of choice:
```
Plug 'gadkadosh/vim-pixem'
```
## How to use it
Running the Ex command 
```
:Pixem
```
will search for any valid values on the current line and convert them from px to em or vice versa.
## How to configure it
Set `g:pixem_base_font_size` to the base px value for the conversion. (Default: 16)  
Set `g:pixem_round_digits` to the number of digits values should be rounded to (em values). (Default: 4)
Set `g:pixem_use_rem` to 1 if you prefer using rem, otherwise use em. (Default: 0)
### Mapping
The plugin does not set a mapping for you. You can add a mapping to your vimrc to your liking, for example:
```
nnoremap <Leader>p :Pixem<CR>
```
## TODO
1. Automatically convert the value for you instead of suggesting only.
2. Work out the edge case of having more than one valid value on the current line.
## Inspiration
I got the idea from https://youtu.be/jKBOhH6EZRg and his plugin https://github.com/joedbenjamin/pixelemconverter
