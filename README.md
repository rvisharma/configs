#Configs

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
