Contributing
============
If you want to contribute to a project and make it better, your help is very welcome. Contributing is also a great way to learn more about social coding on Github, new technologies and and their ecosystems and how to make constructive, helpful bug reports, feature requests and the noblest of all contributions: a good, clean pull request.

### How to make a clean pull request

Look for a project's contribution instructions. If there are any, follow them.

- Create a personal [fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/about-forks) of the project on Github.

<p align="center">
  <img src="https://i.postimg.cc/c1RZJ4Gc/fork-image.png" alt="Highlighting fork button on profile." />
</p>

- Clone the fork on your local machine. Your remote repo on Github is called `origin`.

<p align="center">
	<code>git clone [https://github.com/your-username/contributing.git]</code>
</p>

- Add the original repository as a [remote](https://github.com/git-guides/git-remote) called `upstream`.

<p align="center">
	<code>git remote add upstream https://github.com/[main-profile-name]/[repository-name].git</code>
</p>

- If you created your fork a while ago be sure to pull upstream changes into your local repository.

<p align="center">
	<code>git pull upstream master</code>
</p>

- Create a new branch to work on! Branch from `develop` if it exists, else from `master`.

<p align="center">
	<code>git branch [branch_name]</code>
</p>

- Switch to the newly created brach with:

<p align="center">
	<code>git checkout [branch_name]</code>
</p>

- Implement/fix your feature, comment your code.
- Follow the code style of the project, including indentation.
- If the project has tests run them!
- Write or adapt tests as needed.
- Add or change the documentation as needed.
- Squash your commits into a single commit with git's [interactive rebase](https://help.github.com/articles/interactive-rebase). Create a new branch if necessary.
- Push your branch to your fork on Github, the remote `origin`.

<p align="center">
	<code>git push -u [branch_name]</code>
</p>

- From your fork open a pull request in the correct branch. Target the project's `develop` branch if there is one, else go for `master`!

<p align="center">
  <img src="https://i.postimg.cc/XY1m7XNX/how-to-pull-request.gif" alt="Gif: How to open a pull request on working branch." />
</p>

- If the maintainer requests further changes just push them to your branch. The PR will be updated automatically.
- Once the pull request is approved and merged you can pull the changes from `upstream` to your local repo and delete
your extra branch(es).

And last but not least: Always write your commit messages in the present tense. Your commit message should describe what the commit, when applied, does to the code – not what you did to the code.
