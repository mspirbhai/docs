# Adding a local repository to GitHub using Git

Create a new repository on GitHub.com. To avoid errors, do not initialize the new repository with README, license, or gitignore files. You can add these files after your project has been pushed to GitHub.

Open Git Bash.

Change the current working directory to your local project.

Use the init command to initialize the local directory as a Git repository. By default, the initial branch is called master.

If you’re using Git 2.28.0 or a later version, you can set the name of the default branch using -b.

`$ git init -b main`

If you’re using Git 2.27.1 or an earlier version, you can set the name of the default branch using && git symbolic-ref HEAD refs/heads/main.

`$ git init && git symbolic-ref HEAD refs/heads/main`

Add the files in your new local repository. This stages them for the first commit.
```
$ git add .
# Adds the files in the local repository and stages them for commit. To unstage a file, use 'git reset HEAD YOUR-FILE'.
```

Commit the files that you've staged in your local repository.
```
$ git commit -m "First commit"
# Commits the tracked changes and prepares them to be pushed to a remote repository. To remove this commit and modify the file, use 'git reset --soft HEAD~1' and commit and add the file again.
```

Copy remote repository URL field

In the Command prompt, add the URL for the remote repository where your local repository will be pushed.
```
$ git remote add origin <REMOTE_URL>
# Sets the new remote
$ git remote -v
# Verifies the new remote URL
```

Push the changes in your local repository to GitHub.com.
```
$ git push origin main
# Pushes the changes in your local repository up to the remote repository you specified as the origin

```