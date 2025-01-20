# Initial setup of Mac OS Development Machine

## List of softwares to install

1. Homebrew
2. iTerm2
3. NVM (Node)
4. Yarn
5. Visual Studio Code
6. Oh My Zsh
7. Powerline Fonts

## Installation steps and commands

### Check ZSH version

zsh --version

---

### Install Homebrew

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

---

### Set Homebrew in path

echo '# Set PATH, MANPATH, etc., for Homebrew.' >> /Users/sriramkilambi/.zprofile

echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> /Users/sriramkilambi/.zprofile

eval "$(/opt/homebrew/bin/brew shellenv)"

---

### Check default Shell is set to ZSH

echo $SHELL

---

### Install iTerm2 using brew

brew install iterm2 --cask

---

### Install Node JS using NVM

curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.2/install.sh | bash

nvm install 18.12.1

node -v

npm -v

---

### Install Oh My Zsh

sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

---

### Change theme in ZSHRC

vim .zshrc

ZSH_THEME="agnoster"

Close Vim and Source ZSH

source ~/.zshrc

---

### Download Powerline fonts to get rid of question marks

git clone https://github.com/powerline/fonts.git --depth=1

cd fonts

./install.sh

cd ..

rm -rf fonts

---

### Install MesloLGS Nerd Font Mono

brew install --cask font-meslo-lg-nerd-font

---

### Iterm2 fonts - Select preferred font in iTerm preferences -> Text

Select Font -> MesloLGS Nerd Font Mono

Check Use a different font for non-ASCII text

Select Non-Ascii Font -> MesloLGS Nerd Font Mono

---

### Install Snazzy Theme for iTerm2 and add it to iTerm presets

(curl -Ls https://raw.githubusercontent.com/sindresorhus/iterm2-snazzy/main/Snazzy.itermcolors > /tmp/Snazzy.itermcolors && open /tmp/Snazzy.itermcolors)

---

### Select Snazzy in iTerm preferences -> Colors

Colors -> Load Presets -> Snazzy

---

### Install your favorite ohmyzsh Plugins

git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

Edit in .zshrc

plugins=(git zsh-autosuggestions)

---

### Add your favorite Aliases

alias switchBranch='f() { gf && gco $1 && yarn }; f'

---

### Add prompt to show current date/time

In zshrc -

PROMPT='%{$fg[blue]%} [%D{%f/%m/%y} %D{%L:%M:%S}] '$PROMPT

---

### Setup Default Terminal in VSCode to be iTerm by adding these lines in **_settings.json_**

"terminal.external.osxExec": "iTerm.app",

"terminal.explorerKind": "external",

"terminal.integrated.fontFamily": "MesloLGS Nerd Font Mono"

---

### Install NeoVim

brew install neovim

---

### Install Ripgrep

brew install ripgrep

---

### Install LazyGit

brew install jesseduffield/lazygit/lazygit

---

### Install TMUX

brew install tmux

---

### Install TMUX Plugin Manager

git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm

---
