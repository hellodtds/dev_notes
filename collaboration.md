# Filtering Collaborator's Commits

The git log command is extremely powerful, and you can use it to discover a lot about a repository. But it can be especially helpful to discover information about a repository that you're collaborating on with others. You can use git log to:

1. group commits by author with git shortlog

  `$ git shortlog`

2. filter commits with the --author flag

  `$ git log --author="Richard Kalehoff"`

3. filter commits using the --grep flag

  `$ git log --grep="border radius issue in Safari"`