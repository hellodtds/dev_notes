# Filtering Collaborator's Commits

## Group By Commit Author

 A quick way that we can see how many commits each contributor has added to the repository is to use the `git shortlog` command:

 `$ git shortlog`

## Filter By Author

`$ git log --author=Surma`

Another way that we can display all of the commits by an author is to use the regular git log command but include the --author flag to filter the commits to the provided author.