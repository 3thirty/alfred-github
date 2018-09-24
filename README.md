# alfred-github
Simple alfred workflow to quickly open remote github links to a repository that is checked out locally

## Setup
The following variables must be set in the workflow in Alfred (see https://www.alfredapp.com/help/workflows/advanced/variables/#environment for an example)

| Variable Name | Meaning | Example |
| ------------- | ------- | ------- |
| branch | the github branch to open all links at | `master` |
| giturl | the base URL of the github repository | `https://www.github.com/3thirty/alfred-github` |
| workdir | the working directory that the github repository is checked out to locally | `/Users/ethan/work/alfred-github` |

## Usage
The workflow currently opens 3 types of github URLS:

1. **file** (aka **blob**) - open a file on github (e.g. https://www.github.com/3thirty/alfred-github/blob/master/README.md)
1. **history** (aka **commits**) - open the commit history for a file (e.g. https://www.github.com/3thirty/alfred-github/commits/master/README.md)
1. **blame** - open a file in blame mode (e.g. https://github.com/3thirty/alfred-github/blame/master/README.md)

For **file** and **blame** pressing `cmd+enter` will prompt you for a line number to be highlighted in guthub

## TODOs:
  * [ ] add support for linenumber ranges (e.g. `#L1-L99`)
