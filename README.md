This is my .dotfiles.

Shell is zsh.

Use chezmoi to manage the files between computers.

Use oh-my-zsh for plugins and such.
https://github.com/ohmyzsh/ohmyzsh

Theme:

- https://github.com/sindresorhus/terminal-snazzy
- https://github.com/sindresorhus/iterm2-snazzy

## Prerequisites

- [Brew](https://brew.sh/)

## Install order

Likely in this order anyway. It is the order and method used for the last computer I installed this on (MacBook Air M1 2020).

1. **oh-my-zsh**  
  `sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
2. **zsh-nvm**  
  `git clone https://github.com/lukechilds/zsh-nvm ~/.oh-my-zsh/custom/plugins/zsh-nvm`
3. **zsh-completions**  
  `git clone https://github.com/zsh-users/zsh-completions ${ZSH_CUSTOM:=~/.oh-my-zsh/custom}/plugins/zsh-completions`
4. **Lastpass CLI**  
  for secrets in Chezmoi  
  `brew install lastpass-cli`
5. **autojump**  
  `brew install autojump`
6. **Syntax highlighting**  
  `git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting`
7. **Pure prompt**  
  `git clone https://github.com/sindresorhus/pure.git "$HOME/.zsh/pure"`
  Note: npm install does not work on Apple M1 so that's why we do the git clone.
8. **chezmoi**  
  `chezmoi init --apply bonny`
