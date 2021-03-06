#CodeBlocks
CodeBlock are blocks of code than be assigned to variables and user in operators.
```
{.*}s; 5s o
```

* pushes a CodeBlock to the stack with the contents of `.*`
* the value of `s` is set to the CodeBlock
* the CodeBlock is popped off
* `5` is pushed to the stack
* `s` runs, squaring 5
* `25` is outputted

You can use the [`N` macro](http://o.readthedocs.org/en/latest/spec/macros/) as
shorthand for `{}`.

If a code block is only one character long, you can use `L`. This:

```
{_}:s; 5s o
```

will print `-5`, as will this:

```
L_:s; 5s o
```

`Lc`, where `c` represents any character, will create a code block with the
contents `{c}`.
