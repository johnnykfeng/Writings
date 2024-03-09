# Mastering the Vim Language

These are notes from taken from the contents of this video
https://www.youtube.com/watch?v=wlR5gYd6um0

# Surround Input tricks

`cs` followed by current surrounding bracket and replacement bracket, will change

hello world

(hello world)

# selecting everything inside indents
`ii` targets everything inside an indent block
So combos like `vii` highlights everything of the same indent.
`dii` combo to delete everything in the indent block. Same concept can be applied to other actions such as `y` for yank and `c` for change.


```python
for outer_loop_variable in outer_loop_iterable:
    for inner_loop_variable in inner_loop_iterable:
        # Code to be executed inside the inner loop
        pass

    # Code to be executed after the inner loop completes for each iteration of the outer loop
    pass

```