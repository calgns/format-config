# Format config files
Just to make things easy

quick summary:
- it helps you fix your code
- better indent your code and maintainig the Good habits
- quite simple to use

all of this so it will be almost no common errors.

if you don't undestand what each one of the format file does, then, go to the end of this file and click the link of the one you didn't undestand.

## Overview :owl:
Here will be most common config files.

Includes:

- `eslint`
  - `babel-eslint`
  - `eslint-plugin-react`
  - `eslint-plugin-react-hooks`

- `editorconfig`
- `stylelint`
- `prettier`

## Setup 🏖️

simply follow the commands and finally have fun.

clone the repo

```sh 
git clone https://github.com/calgns/format-config
cd ./format-config
```

basically move the files into _YourDir_ and delete this directory.
_OBS: change YourDir so you actually put a dir that you are working on._
```sh 
mv .prettierrc.js .eslintrc.js .editorconfig .stylelintrc.json ../?YourDir?
```

 if you're using a project that has jsx and tsx mixed or an old project that is going to use ts
```sh
mv .eslintrc.json 
rm ~/?YourDir?/.eslintrc.js
```

remove this dir while inside of it
```sh
rm -fr ../format-config
```

now in your dir run
```sh
# if you have pnpm good
pnpm i eslint@latest prettier@latest stylelint@latest babel/eslint-parser@latest eslint-plugin-react@latest eslint-plugin-react-hooks@latest stylelint-config-standard@latest -D


# if don't, you should, cause it's like npm but with some goods
npm i eslint@latest prettier@latest stylelint@latest babel/eslint-parser@latest eslint-plugin-react@latest eslint-plugin-react-hooks@latest stylelint-config-standard@latest -D
```


## Usage on vscode
### first exemple simple one in js file
![First gif exemple vscode js file](./assets/md-exemple.gif)
### second exemple more complex one in large jsx file
![second gif exemple vscode large js file](./assets/md-exemple2.gif)
### third exemple simple one in css file
![third gif exemple vscode css file](./assets/md-exemple3.gif)

## Usage on terminal
if in your settings you have chosen to format on save and if have errolens installed you will rarely see the terminal.

inside the root of the project

### eslint
```sh
# you have to specify if it's a js or jsx file
npx eslint src/**/*.jsx
```

### prettier
```sh
# this will normally output what it should be written
npx prettier src/app/layout.js 

# check the file so you can see if it's pretty 
npx prettier -c src/app/layout.js 

# check all the files
npx prettier -c src/**/*.jsx 

# formats the file
npx prettier -w src/app/layout.js 

# manual so you can do lots of things
npx prettier -h
```

### stylelint
```sh
# checks all css files and has a nice output
npx stylelint src/**/*.css
```

## How it should look on terminal
### running commands
![GifExempleTerminal](./assets/md-exemple4.gif)

## Don't forget
if you want it to work correctly then you should download each one extension in vscode and always explore the docs.

### [eslint](https://eslint.org/) [stylelint](https://stylelint.io/) [prettier](https://prettier.io/) [editorconfig](https://editorconfig.org/) 

