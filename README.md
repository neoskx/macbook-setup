# Mackbook Setup for an Engineer
> Mackbook setup for front-end engineer, backend engineer, and full-stack engineer

## System Preferences
Set system preferences by the terminal

### Show library folder
`chflags nohidden ~/Library` 
### Show hidden files
`defaults write com.apple.finder AppleShowAllFiles YES`
### Show path bar
`defaults write com.apple.finder ShowPathbar -bool true`
### Show status bar
`defaults write com.apple.finder ShowStatusBar -bool true`
### Show items as column
`defaults write com.apple.finder FXPreferredViewStyle clmv`

After running those commands, run `killall Finder`

## Terminal Tools

### [oh my zsh](https://ohmyz.sh/)
Unleash your terminal like never before
**Install**
`sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
#### Plugins
Oh My Zsh comes bundled with [plugins](https://github.com/ohmyzsh/ohmyzsh/wiki/Plugins)

Enable following plugins
* **git**
* **[zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)**
  `git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting`
* **[zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions)**
  `git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions`
* **[zsh-completions](https://github.com/zsh-users/zsh-completions)**
  `git clone https://github.com/zsh-users/zsh-completions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-completions`

### [Howebrew](https://brew.sh/)
The Missing Package Manager for macOS (or Linux)
**Install**
`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
