This is my .dotfiles.

Shell is zsh.

Use chezmoi to manage the files between computers.

Use oh-my-zsh for plugins and such.
https://github.com/ohmyzsh/ohmyzsh

Theme:

- https://github.com/sindresorhus/terminal-snazzy
- https://github.com/sindresorhus/iterm2-snazzy

## Some things must be installed:

- **oh-my-zsh**  
  `sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"`
- **zsh-nvm**  
  `git clone https://github.com/lukechilds/zsh-nvm ~/.oh-my-zsh/custom/plugins/zsh-nvm`
- **zsh-completions**  
  `git clone https://github.com/zsh-users/zsh-completions ${ZSH_CUSTOM:=~/.oh-my-zsh/custom}/plugins/zsh-completions`
- **Lastpass CLI**  
  for secrets in Chezmoi  
  `brew install lastpass-cli`
- **autojump**  
  `brew install autojump`
- **Syntax highlighting**  
  `git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting`
- **Pure prompt**  
  `npm install --global pure-prompt`
- **chezmoi**  
  `chezmoi init --apply bonny`
