 export PATH=~/.npm-global/bin:$PATH                                                                                                     
   1 
   2 # Path to your oh-my-zsh installation.
   3 export ZSH="/Users/juan/.oh-my-zsh"
   4 
   5 ZSH_THEME="robbyrussell"
   6 
   7  DISABLE_AUTO_TITLE="true"
   8 
   9 plugins=(git vi-mode)
  10 
  11 source $ZSH/oh-my-zsh.sh
  12 
  13  alias zsh="vim ~/.zshrc"
  14  alias vi="vim ~/.vimrc"
  15  alias t="touch"
  16  alias m="mkdir"
  17  alias l="ls -a"
  18  alias c="clear"
  19  alias r="rm -rf"
  20  alias v="vim"
  21 
  22  bindkey -M viins ' i' vi-cmd-mode
  23 
  24 
  25  zle-line-init() {
  26  zle -K vicmd;
  27 }
  28  zle -N zle-line-init
  29 
  30  export KEYTIMEOUT=10
