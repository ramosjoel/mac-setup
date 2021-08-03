# Mac Setup

## Homebrew
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
brew update
```

## iTerm2
```
brew cask install iterm2
```

## Alfred
```
brew cask install alfred
```

## Slack
```
brew cask install slack
```

## Mas - Apple Store app installs
```
brew install mas
```

## Browsers
```
brew cask install google-chrome
brew cask install brave-browser
brew cask install firefox
```
## Amazon photos
```
brew cask install amazon-photos
```

## Spotify
```
brew cask install spotify
```

## Postman
```
brew cask install postman
```

## Microsoft Office
```
brew cask install microsoft-office
```

## Zoom
```
brew cask install zoomus
```

## VS Code
```
brew cask install visual-studio-code
```

## Terminal utilties
```
brew install jq
brew install tree
brew install wget
```

## Charles Proxy
```
brew cask install charles
```

## Python3
```
brew install python3
```

## Pycharm
```
brew cask install pycharm
```

## Git
```
brew install git
```

## Tmux
```
brew install tmux
```

## ZSH
```
brew install zsh-completions zsh-syntax-highlighting zsh-autosuggestions
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

## dotfiles
```
brew install rcm
./.dotfiles/install.sh
```

## nvm
```
echo "You might want to check for a newer version of nvm."
echo "About to install v0.35.3..."
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash
nvm install --lts
```

## Yarn
```
brew install yarn
```

## Typescript - tsc
```
yarn global add typescript
```

## eslint
```
yarn global add eslint
```

## Powerline status bar
```
# install powerline status bar
pip3 install powerline-status

# install fonts
git clone git@github.com:powerline/fonts.git
cd fonts
./install.sh

# add powerline status bar to ZSH
powerline_root=$(pip3 show powerline-status | grep Location | awk '{print $2}')
# . ${powerline_root}/powerline/bindings/zsh/powerline.zsh
# add powerline status bar to tmux
echo "source ${powerline_root}/powerline/bindings/tmux/powerline.conf" >> .tmux.conf
echo "# ZSH - start tmux when launching iterm windows" >> .zshrc
echo "ZSH_TMUX_AUTOSTART=true" >> .zshrc
```

## Java
```
brew tap adoptopenjdk/openjdk
# run brew search jdk to see available jdks
brew cask install adoptopenjdk14
java -version
```

## Things 3
```
mas install 904280696
```
