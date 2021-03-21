This is my .dotfiles.

Shell is zsh.

Use chezmoi to manage the files between computers.

Use oh-my-zsh for plugins and such.
https://github.com/ohmyzsh/ohmyzsh

Theme:

- https://github.com/sindresorhus/terminal-snazzy
- https://github.com/sindresorhus/iterm2-snazzy

## Some things must be installed:

- _Lastpass CLI_  
  for secrets in Chezmoi  
  `brew install lastpass-cli`
- chezmoi  
  `chezmoi init --apply bonny`
- Pure prompt.  
  `$ npm install --global pure-prompt`
- Syntax highlighting:  
  `$ git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting`
- zsh-completions. 
  https://github.com/zsh-users/zsh-completions
