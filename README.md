# Configs

## Step 0
install xcode command line tools from [here](https://developer.apple.com/download/all/?q=command%20line%20tools)


## Step 1 - Move configs to `~`
- move `.p10k.zsh`
- move `.zshrc`

## Step 1.1 - For intel mac only
> https://docs.brew.sh/Installation
> This script installs Homebrew to its preferred prefix (/usr/local for macOS Intel, /opt/homebrew for Apple Silicon and /home/linuxbrew/.linuxbrew for Linux) so that you don’t need sudo when you brew install.

- in `.zshrc` replace `/opt/homebrew` to `/usr/local`

## Step 2 - Install packages

**Brew**
- cd to this Repo
- exec `brew bundle install`

### Brew bundle commands
- to dump new Brewfile `brew bundle dump`
- to check if all of Brewfile is installed `brew bundle check`

## Step 3 - Karabiner setup
- move `karabiner.json` to `~/.config/karabiner`

## Step 4 - Espanso setup
- copy `espanso` folder content to location `$(espanso path)` -> config
- run `espanso register`

## Step 5 - Setup multiple git configs

[Source - Multiple Accounts and Git](https://www.bram.us/2021/09/03/multiple-accounts-and-git/)

    Here’s an example ~/.gitconfig that has two dynamic includes:

    [user]
      name = "John Doe"

    [includeIf "gitdir:~/repos/personal/"]
      path = ~/.gitconfig.personal

    [includeIf "gitdir:~/repos/work/"]
      path = ~/.gitconfig.work


    Inside each ~/.gitconfig.XXX you can then list extra config values, here the email address to use for each:

    [user]
      email = john@example.org
