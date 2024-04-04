# Mac Setup

## Suggested

### Homebrew
```
# /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
(echo; echo 'eval "$(/opt/homebrew/bin/brew shellenv)"') >> /Users/joel/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
brew update
```

### iTerm2
```
brew install iterm2 --cask
```

### Rectangle (window management)
```
brew install rectangle --cask 
```

### Alfred
```
brew install alfred --cask
```

### Slack
```
brew install slack --cask
```

### Mas - Apple Store app installs
```
brew install mas
```

### Browsers
```
brew install google-chrome --cask
brew install brave-browser --cask
brew install firefox --cask
```

### Amazon photos (not used)
```
# brew install amazon-photos --cask
```

### Spotify
```
brew install spotify --cask 
```

### Postman
```
brew install postman --cask
```

### Microsoft Office (not used)
```
# brew install microsoft-office --cask
```

### Zoom
```
brew install zoomus --cask
```

### VS Code
```
brew install visual-studio-code --cask
```

### Terminal utilties
```
brew install jq
brew install tree
brew install wget
```

### Charles Proxy
```
# brew install charles --cask
```

### Python3
```
brew install python3
```

### Pycharm (no used)
```
# brew install pycharm --cask
```

# ***** CLI Tools ***** #
### Git
```
brew install git
```

### Tmux
```
brew install tmux
```

### fzf
```
brew install fzf     # https://github.com/junegunn/fzf?tab=readme-ov-file#using-homebrew 
brew install bat     # https://github.com/sharkdp/bat?tab=readme-ov-file#on-macos-or-linux-via-homebrew
# brew install exa     # https://the.exa.website/ # disabled by homebrew as "not maintained upstream"
brew install lsd     # https://github.com/lsd-rs/lsd
brew install zoxide  # https://github.com/ajeetdsouza/zoxide?tab=readme-ov-file#installation
```

### ZSH
```
brew install zsh-completions
brew install zsh-autosuggestions
brew install zsh-syntax-highlighting
# brew install zsh-completions zsh-syntax-highlighting zsh-autosuggestions
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

### dotfiles
```
PREVIOUS=${PWD}
cd
git clone git@github.com:ramosjoel/dotfiles.git
mv dotfiles .dotfiles
cd $PREVIOUS
brew install rcm
cd
rcup
cd $PREVIOUS
```

### nvm
```
echo "You might want to check for a newer version of nvm."
echo "About to install v0.39.7..."
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
nvm install --lts
```

### Yarn
```
brew install yarn
```

### Typescript - tsc
```
brew install typescript
```

### eslint
```
yarn global add eslint
```

### Powerline status bar
```
# install powerline status bar
pip3 install powerline-status --break-system-packages
```

### Install fonts
```
git clone git@github.com:powerline/fonts.git
cd fonts
./install.sh
cd ..
rm -rf fonts
```

### add powerline status bar to ZSH
```
PREVIOUS=${PWD}
powerline_root=$(pip3 show powerline-status | grep Location | awk '{print $2}')
echo "powerline stuff should be in ${powerline_root}"
# . ${powerline_root}/powerline/bindings/zsh/powerline.zsh
# [THE BELOW SHOULD NOT BE NEEDED SINCE DOTFILES ARE IN VERSION CONTROL] add powerline status bar to tmux
# echo "source ${powerline_root}/powerline/bindings/tmux/powerline.conf" >> ~/.tmux.conf
# echo "# ZSH - start tmux when launching iterm windows" >> ~/.zshrc
# echo "ZSH_TMUX_AUTOSTART=true" >> ~/.zshrc
cd $PREVIOUS
```

### Java
```
brew tap adoptopenjdk/openjdk
# run brew search jdk to see available jdks
brew install adoptopenjdk14 --cask
java -version
```

### Things 3
```
mas install 904280696
```

### Neovim
```
xcode-select --install
brew install --HEAD tree-sitter
brew install --HEAD luajit
brew install --HEAD neovim
```

## OPTIONAL
Comment these out if they aren't needed

### Kubernetes (k8s)
```
brew install kubectl
brew install helm
```

```
brew install tilt   # (https://docs.tilt.dev/) Tool for managing Kubernetes environments.
brew install kind   # (https://kind.sigs.k8s.io/) Tool for running local Kubernetes clusters.
brew install ctlptl # (https://github.com/tilt-dev/ctlptl/blob/main/docs/ctlptl.md) Tool for managing k8s clusters.
```

### gRPC
```
brew install grpcurl
```

### AWS
```
brew install awscli
```

### AWS LocalStack
```
brew install localstack/tap/localstack-cli # (https://github.com/localstack/localstack) 
# provides the awslocal command, which is a thin wrapper around the aws command line interface for use with LocalStack.
brew install awscli-local # (https://github.com/localstack/awscli-local?tab=readme-ov-file)
```

### Protobuf
```
brew install protobuf
```
