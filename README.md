# dotfiles

Analytics Engineering dotfiles for an M1 Mac

## Setup Steps

Open your new mac and go through all the setup screens - this takes a little while. Once complete, you'll need [iTerm2](https://iterm2.com/).

When I did this, I got notified that I needed to install:

* Developer tools
* Message about installing pip3
Let's hope neither of those cause problems later

Open applications in Finder. Using the options menu in the top right or a right click, open the menu for iTerm and select `Duplicate`. On the new copy, select `Get Info` and check the option to `Open using Rosetta`. You'll be prompted to install Rosetta.

## Git Setup

If you try to run the script as is, you'll get the following error when you try to sign in to github:
`remote: Support for password authentication was removed on August 13, 2021. Please use a personal access token instead.`

To fix this:

1. Generate a PAT [instructions](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)
2. Enter it instead of your password when prompted on the command line

Resolved this by making it public - entering the PAT by copying and pasting into the command line did not work.

## Run the Setup Script

I pasted it straight into the iTerm2 terminal.

## Open VS Code

In theory, this part should be doable by adding the VS Code path to the `.zshrc` file.
To get my extensions out of VS Code on my old mac I used the [menu option](https://stackoverflow.com/questions/29955500/code-not-working-in-command-line-for-visual-studio-code-on-osx-mac) to add it to the path.

### Command Line Extension Management

* [VS Code Help Docs](https://code.visualstudio.com/docs/editor/extension-marketplace#_command-line-extension-management)
* [Parse each line of a text file as an arguement to a command](https://unix.stackexchange.com/questions/149726/how-to-parse-each-line-of-a-text-file-as-an-argument-to-a-command)
* To export extensions to this repo use `code --list-extensions > vscode-extensions.txt`
