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

## Terminal Applications

### [Howebrew](https://brew.sh/)
The Missing Package Manager for macOS (or Linux)

**Install**

`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

### [nerd-fonts](https://github.com/ryanoasis/nerd-fonts)

**Install**

`brew install font-hack-nerd-font`

### [oh my zsh](https://ohmyz.sh/)
Unleash your terminal like never before

**Install**

`sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`

#### Theme
Recommend to use [Starship]()

**Install**

`brew install starship`

Add to `.zshrc`: 

`echo 'eval "$(starship init zsh)"' >> ~/.zshrc`

Use [Nerd Font Symbols Preset](https://starship.rs/presets/nerd-font):

`starship preset nerd-font-symbols -o ~/.config/starship.toml`

> Select **Hack Nerd Font**
> 
> iTerm
> 
> <img width="1011" alt="image" src="https://github.com/neoskx/macbook-setup/assets/870358/659d7958-aff2-486c-894c-ad8f1304398d">

> Terminal
> 
> <img width="779" alt="image" src="https://github.com/neoskx/macbook-setup/assets/870358/ff131ef2-6015-44c4-8557-bb86ebdd0b04">


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
* **[colored-man-pages](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/colored-man-pages)**
 
```
plugins=(
  git
  colored-man-pages
  zsh-autosuggestions
  zsh-syntax-highlighting
  zsh-completions
)
```

## Applications
### [iTerm2](https://iterm2.com/)
iTerm2 is a replacement for Terminal and the successor to iTerm. 
### [Visual Studio Code](https://code.visualstudio.com/)
Code editing. Redefined. Free. Built on open source. Runs everywhere.
### [Docker](https://www.docker.com/products/docker-desktop/)
Accelerate how you build, share, and run applications

## Development Environment 
### NodeJS
#### [nvm](https://github.com/nvm-sh/nvm)
Node Version Manager

**Install**

`curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash`

#### [yarn](https://yarnpkg.com)
Yarn is a package manager that doubles down as project manager.

### Python
#### [pyenv](https://github.com/pyenv/pyenv)
Simple Python version management

**Install**

`brew install pyenv`

```shell
echo 'export PYENV_ROOT="$HOME/.pyenv"' >> ~/.zshrc
echo '[[ -d $PYENV_ROOT/bin ]] && export PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.zshrc
echo 'eval "$(pyenv init -)"' >> ~/.zshrc
```

