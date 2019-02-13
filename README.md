When copying/pasting from the term into :e from the output of tests, linters or
other tools, we often have output like this

```
spec/services/foo_spec.rb:39:7: C: Style/StringLiterals: Prefer single-quoted strings ...
```

I want to double click the filename and copy/paste it into an `:edit` command.
This would result in the following:

```
:e spec/services/foo_spec.rb:39:7:
```

Now I would have to strip off the `:39:7:`. Or we could just get vim to
interpret this properly and open the file at line 39. Thats what this plugin
does.

