## Adding ESLint to VSC

## Adding ESLint to pre-commit hooks
There are manly two ways to add your pre-commit hooks, manualy or automatically. Automatic is good if you want to forget what is going behind the scenes, whereas manually you have a higher level of control to which hook(s) you desire adding to git, and their functionality.

### Automatically
There is an npm package called husky that will add automaticly a precommit hook to package.json. To add it run npm install husky --save-dev
An interesting feature that this package comes with is the ability to bypass it, for that you just need to add the --no-verify flag as in:
git commit -m "A very ignorant commit" --no-verify

### Manualy adding it
- 1 - Initialize git
- 2 - Go to .git/hooks and rename pre-commit.sample to pre-commit as instructed.
- 3 - Change existing code to become only the code found in the [link](https://gist.github.com/rashtay/328da46a99a9d7c746636df1cf769675
).
- 4 - Finally make sure your file is executable, if it isn't change the execute(x) permission.
