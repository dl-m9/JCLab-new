# JC STEM Lab for Smart City

This is the official website of JC STEM Lab for Smart City

## Get Started

Prerequisite:
- Go
- Git
- Node.Js

### Mac
If you want to know how to get started in Windows or Linux, check the [document of wowchemy](https://wowchemy.com/docs/getting-started/install-hugo-extended/).
- Open the Terminal App
- Install HomeBrew
``` bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```

- Apply any Homebrew updates

```bash
brew update && brew upgrade
```
- Install dependencies
```bash

brew install git golang hugo node

```

- Open `~/.zshrc`(or `~/.bashrc`)
```shell
export PATH=$PATH:/usr/local/go/bin >> ~/.zshrc
```
- View the site:

```shell
hugo server
```