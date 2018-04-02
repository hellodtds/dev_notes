# Filtering Collaborator's Commits

## Group By Commit Author

 A quick way that we can see how many commits each contributor has added to the repository is to use the `git shortlog` command:

 `$ git shortlog` displays an alphabetical list of names and the commit messages that go along with them.


_We can add a couple of flags:_
`$ git shortlog -s -n`

1. -s to show just the number of commits (rather than each commit's message)
2. -n to sort them numerically (rather than alphabetically by author name)

```
910  Paul Irish
360  Brendan Kenny
244  Patrick Hulce
238  Eric Bidelman
154  Paul Lewis
148  Sam Saccone
```


