# What is aliases ?

- Aliases allow you to save your pipelines and commands with easy to remember nicknames so that they can be used later much easier.

- You define aliases in your `.bash_aliases` file in your home directory.

- Here is how you define an alias in `.bash_aliases`:

`alias aliasName=”THING YOU WANT TO ALIAS”`

> Note: there are no space between the equal sign and the quote ("") and the aliasName. the quotes must be single quotes or double quotes.

- Example: 
```
alias calmagic="cal -A 1 -B 1 12 2017"
```

- With this alias defined in our `.bash_aliases` file, whenever we run the `calmagic` command it is as if we ran the `cal –A 1 –B 1 12 2017` command.

- `calmagic` is now said to be an alias of `cal –A 1 –B 1 12 2017`

- **Piping to an alias**

- If the `first` command in an alias accepts the standard input, then the alias can be piped to, even if it is an entire pipeline.

- 
