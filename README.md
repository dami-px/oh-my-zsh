# oh-my-zsh
 
https://ohmyz.sh/#install

code ~/.zshrc


plugins=(git direnv nvm zsh-autosuggestions zsh-syntax-highlighting zsh-completions)

git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions

brew install zsh-syntax-highlighting

echo "source $(brew --prefix)/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> ${ZDOTDIR:-$HOME}/.zshrc

https://github.com/zsh-users/zsh-completions?tab=readme-ov-file#oh-my-zsh



zstyle ':omz:plugins:nvm' autoload yes
zstyle ':omz:plugins:nvm' silent-autoload true

autoload -U compinit && compinit

source $ZSH/oh-my-zsh.sh