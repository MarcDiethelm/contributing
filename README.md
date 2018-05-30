Contributing
============
If you want to contribute to a project and make it better, your help is very welcome. Contributing is also a great way to learn more about social coding on Github, new technologies and and their ecosystems and how to make constructive, helpful bug reports, feature requests and the noblest of all contributions: a good, clean pull request.

### How to make a clean pull request

Look for a project's contribution instructions. If there are any, follow them.

- Create a personal fork of the project on Github.
- Clone the fork on your local machine. Your remote repo on Github is called `origin`.
```
git clone < your_forked_repo >
git remote -v
```
- Add the original repository as a remote called `upstream`. Select branch_in_original_repo as `develop` if it exists, else go for `master`.
```
git remote add upstream < original_repo_from_which_you_forked / branch_in_original_repo >
```
- If you created your fork a while ago be sure to pull upstream changes into your local repository.
```
git pull upstream
```
- Create a new branch to work on! Branch from `develop` if it exists, else from `master`.
```
git checkout < branch_in_original_repo >
git checkout -b < your_new_branch >
```
- Implement/fix your feature, comment your code.
```
git status
git add .
git commit -m 'your_commit' or git commit -S -m 'your_commit' for signed commit
```
- Follow the code style of the project, including indentation.
- If the project has tests run them!
- Write or adapt tests as needed.
- Add or change the documentation as needed.
- Squash your commits into a single commit with git's [interactive rebase](https://help.github.com/articles/interactive-rebase). Create a new branch if necessary.
- Push your branch to your fork on Github, the remote `origin`.
```
git push --set-upstream origin < your_new_branch >
```
- From your fork open a pull request in the correct branch. Target the project's `develop` branch if there is one, else go for `master`!
```
In Github page of your repo, you will have this option.
```
- …
- If the maintainer requests further changes just push them to your branch. The PR will be updated automatically.
- Once the pull request is approved and merged you can pull the changes from `upstream` to your local repo and delete
your extra branch(es).
```
git branch -d < your_new_branch >  if merged
git branch -D < your_new_branch >  force delete
```

And last but not least: Always write your commit messages in the present tense. Your commit message should describe what the commit, when applied, does to the code – not what you did to the code.
