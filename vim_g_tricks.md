This blog is based on Luke Smith's video on Vim tips
https://www.youtube.com/watch?v=bQfFvExpZDU
very handy, highly recommended

## Movement commands with "g" modifier
When a line is long and continous, it may wrapped, then appearing as several visual lines on the editor, but is recognized as one line in Vim. Using standard `j` and `k` up and down movements will treat them as one line, thus skipping a bunch of text. Use the `g` modifier to actually treat them as individual lines. 
`gj`,`gk`, `g0`, `g$`. 

But even better, is to use to auto-format the long line into several Vim lines. To do that, use `gq` followed by a movement. `gq` behaves like commands such as `d`, `y`, and `c`, where they must be followed by another command that instructs it how and where to apply the action.


## captilalization
`gu`
`gu`
`~` swithes the capitalization
Coding_Vim_Keybindings.md

## go to file
`gf`

## conjoining lines

`J` conjoin lines with space in between
`gJ` conjoin lines without space

## substitution
When I was taught substitution, I commonly see `:%s/<old_word>/<new_word>`, which substitutes `old_word` for `new_word`, follow that with `/g` if you want to substitute for entire document, or `/gc` to do ask confirmation at each occurence, or `/gi` for case insensitive substitution.

However, less common is applying the substitution on a single line
`:s/<old_word>/<new_word>`
After that, I can then use `g&` to apply the same substitution to the entire document. This is a great way to test the substitution before applying it to the entire document.

nebulae


### Lorem ipsum for practice

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.  Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
tempor incididunt ut labore et dolore magna aliqua. Vestibulum sed arcu non
odio euismod lacinia at quis risus. A iaculis at erat pellentesque
adipiscing commodo. Lobortis elementum nibh tellus molestie nunc non. Est
lorem ipsum dolor sit amet consectetur adipiscing elit. Justo nec ultrices
dui sapien eget mi proin. Pretium quam vulputate dignissim suspendisse in
est ante. Est sit amet facilisis magna etiam. Massa enim nec dui nunc.
Turpis egestas maecenas pharetra convallis posuere morbi.

