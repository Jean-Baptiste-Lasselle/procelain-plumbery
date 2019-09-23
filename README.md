# Pocoelain or Plumbery
What's the difference between porcelain and plumbery in Git? 

https://stackoverflow.com/questions/424071/how-to-list-all-the-files-in-a-commit

```bash 
# Preferred Way (because it's a plumbing command; meant to be programmatic):

$ git diff-tree --no-commit-id --name-only -r bd61ad98
index.html
javascript/application.js
javascript/ie6.js

# Another Way (less preferred for scripts, because it's a porcelain command; meant to be user-facing)

$ git show --pretty="" --name-only bd61ad98    
index.html
javascript/application.js
javascript/ie6.js

```
