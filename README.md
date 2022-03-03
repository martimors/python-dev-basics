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

# Setting up a Python environment and debugging in VSCode

## Create a python 3 virtual environment

Make sure you have python version 3.x installed, then do

```
python3 -m venv venv
```

## Open current folder in VScode

```
cd my/folder
code .
```

## Ignore the venv files in git

It makes no sense to track your venv. To ignore it, make a file called
`.gitignore`, and write `venv` in it.

## Select the python interpreter in VSCode

Open the command pallette with shift+command+P (or shift+ctrl+P on linux), then look for the command `Python: Select Interpreter`. Pick the venv that you just created in the previous step. The VSCode debugger will use this venv.

## Make a basic python script and debug it

Create a file called `main.py` (or whatever you want), and write some code in it:

```python
def power(a, b):
    return a**b


print("hello world")

c = power(10, 3)

print(c)
```

While having this file open in VSCode, press F5 to start the debugger. If prompted, select "Current file". This will run your script.

You can also add a breakpoint by clicking in the left margin of the file. The debugger will stop when it encounters a breakpoint.

To go to the next line, press F10. To step into a function, press F11.
