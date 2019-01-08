Contributing
============
If you want to contribute to a project and make it better, your help is very welcome. Contributing is also a great way to learn more about social coding on Github, new technologies and and their ecosystems and how to make constructive, helpful bug reports, feature requests and the noblest of all contributions: a good, clean pull request.

### How to make a clean pull request

Look for a project's contribution instructions. If there are any, follow them.

1. Create a personal fork of the project on Github.
```bash
Click the fork-button on the project page on Github.
```
2. Clone the fork on your local machine. Your remote repo on Github is called `origin`.
```bash
git clone https://github.com/user/fork.git
```
3. Add the original repository as a remote called `upstream`.
```bash
git remote add upstream https://github.com/original/project.git
```
4. If you created your fork a while ago be sure to pull upstream changes into your local repository.
```bash
git pull upstream master
```
5. Create a new branch to work on! Branch from `develop` if it exists, else from `master`.
```bash
git checkout -b <branchname>
```
6. Implement/fix your feature, comment your code.
```bash
git add // git commit -m
```
7. Follow the code style of the project, including indentation.
8. If the project has tests run them!
9. Write or adapt tests as needed.
10. Add or change the documentation as needed.
11. Squash your commits into a single commit with git's [interactive rebase](https://help.github.com/articles/interactive-rebase). Create a new branch if necessary.
```bash
git rebase --interactive gitexamples
use s (squash on all commits except the first one and change the commit message.)
```
12. Push your branch to your fork on Github, the remote `origin`.
```bash
git push remote master 
```
13. From your fork open a pull request in the correct branch. Target the project's `develop` branch if there is one, else go for `master`!
14. …
15. If the maintainer requests further changes just push them to your branch. The PR will be updated automatically.
16. Once the pull request is approved and merged you can pull the changes from `upstream` to your local repo and delete
your extra branch(es).

And last but not least: Always write your commit messages in the present tense. Your commit message should describe what the commit, when applied, does to the code – not what you did to the code.
