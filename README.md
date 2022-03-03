# Basic version control

## Creating a GIT repository

```
mkdir my-project
cd my-project
git init
```

## Making a commit

```
touch README.md  # Make a file
git add .
git commit -m "My awesome message"
```

You can always check the status in your repository by typing `git status`.

## Push the local commits to remote (fx. GitHub)

```
git remote add origin <URL to repo>
git push
```

## Get remote commits to local

```
git pull
```
