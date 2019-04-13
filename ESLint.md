## ESLint in VSC
You can integrate ESLint to VSC by downloading [this extension](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint) that integrates ESL, the only prerequisite for it to work is having ESLint in your machine. 

They also state a useful piece of information: "On new folders you might also need to create a .eslintrc configuration file. You can do this by either using the VS Code command Create ESLint configuration or by running the eslint command in a terminal. If you have installed ESLint globally (see above) then run eslint --init in a terminal. If you have installed ESLint locally then run .\node_modules\.bin\eslint --init under Windows and ./node_modules/.bin/eslint --init under Linux and Mac.
"

## Adding ESLint to pre-commit hooks
There are manly two ways to add your pre-commit hooks, manually or automatically. Automatic is good if you want to forget what is going behind the scenes, whereas manually is good for these who want to have a higher level of control.

### Automatically
If you desire to add automatically there is an npm package called husky that will make your life easier by turning adding pre-commit hooks into a declarative task. There is a great [blog post](https://medium.com/netscape/git-hooks-with-husky-8b98f2556363) about how to use it effectively.

### Manualy adding it

To add it manyally just follow the four simple steps:
- 1 - Initialize git
- 2 - Go to .git/hooks and rename pre-commit.sample to pre-commit as instructed.
- 3 - Change existing code to become your pre-commit hook, or copy the code found in the [link](https://gist.github.com/rashtay/328da46a99a9d7c746636df1cf769675
).
- 4 - Finally make sure your file is executable, if it isn't change the execute permission.
