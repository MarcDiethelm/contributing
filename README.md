Contributing
============
If you want to contribute to a project and make it better, your help is very welcome. Contributing is also a great way to learn more about social coding on Github, new technologies and and their ecosystems and how to make constructive, helpful bug reports, feature requests and the noblest of all contributions: a good, clean pull request.

### How to make a clean pull request

Look for a project's contribution instructions. If there are any, follow them.

{note} The bash commands below will give you step-by-step intructions to contribute to this Contributing project.

- Create a personal fork of the project on Github.
- Clone the fork on your local machine. Your remote repo on Github is called `origin`.

```bash
#To clone your fork into a folder called Contributing
git clone git@github.com:cbernard73/contributing.git Contributing2
```

- Add the original repository as a remote called `upstream`.

```bash
#To add the original repo as a remote called upstream
git remote add upstream git@github.com:MarcDiethelm/contributing.git
```

- If you created your fork a while ago be sure to pull upstream changes into your local repository.

```bash
#To pull any recent updates
git pull upstream master
```

- Create a new branch to work on! Branch from `develop` if it exists, else from `master`.

```bash
#To create a new local branch and switch to that branch
git checkout -b fb-command-line-examples
```

- Implement/fix your feature, comment your code.

```bash
#To make your first change
vi README.md
git add README.md
git commit -m "Add bash commands to steps"

#Make another change
vi README.md
git add README.md
git commit -m "Add more bash commands to even more steps"

#Results in two commits to your fork of the repo
```

- Follow the code style of the project, including indentation.
- If the project has tests run them!
- Write or adapt tests as needed.
- Add or change the documentation as needed.
- Squash your commits into a single commit with git's [interactive rebase](https://help.github.com/articles/interactive-rebase). Create a new branch if necessary.

```bash
#To combine the changes from the previous two commits
git reset --soft HEAD~2

#To commit the combined changes and create a new message
git commit -m "Add bash commands to steps"
```

- Push your branch to your fork on Github, the remote `origin`.

```bash
git push --set-upstream origin fb-command-line-examples
```

- From your fork open a pull request in the correct branch. Target the project's `develop` branch if there is one, else go for `master`!
- …
- If the maintainer requests further changes just push them to your branch. The PR will be updated automatically.
- Once the pull request is approved and merged you can pull the changes from `upstream` to your local repo and delete
your extra branch(es).

And last but not least: Always write your commit messages in the present tense. Your commit message should describe what the commit, when applied, does to the code – not what you did to the code.
