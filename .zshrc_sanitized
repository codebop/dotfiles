# If you come from bash you might have to change your $PATH.
export PATH=$HOME/bin:/usr/local/bin:$PATH

# Path to your oh-my-zsh installation.
export ZSH=/Users/danquinn/.oh-my-zsh

# Set name of the theme to load. Optionally, if you set this to "random"
# it'll load a random theme each time that oh-my-zsh is loaded.
# See https://github.com/robbyrussell/oh-my-zsh/wiki/Themes

ZSH_THEME="powerlevel9k/powerlevel9k"

POWERLEVEL9K_ALWAYS_SHOW_USER='false'
POWERLEVEL9K_MODE='nerdfont-complete'
export DEFAULT_USER="$USER"

# Which plugins would you like to load? (plugins can be found in ~/.oh-my-zsh/plugins/*)
# Custom plugins may be added to ~/.oh-my-zsh/custom/plugins/
# Example format: plugins=(rails git textmate ruby lighthouse)
# Add wisely, as too many plugins slow down shell startup.
plugins=(
  git
)

source $ZSH/oh-my-zsh.sh

#
# Example aliases
# alias zshconfig="mate ~/.zshrc"
#alias ohmyzsh="mate ~/.oh-my-zsh"
POWERLEVEL9K_LEFT_PROMPT_ELEMENTS=(context dir aws pyenv rbenv vcs ssh)
POWERLEVEL9K_RIGHT_PROMPT_ELEMENTS=(status root_indicator background_jobs history time)
POWERLEVEL9K_PROMPT_ON_NEWLINE=true
POWERLEVEL9K_RPROMPT_ON_NEWLINE=true
su() {
  sudo -sE
}
# rbenv
eval "$(rbenv init -)"

# pyenv | virtualenv
eval "$(pyenv init -)"
eval "$(pyenv virtualenv-init -)"
export PYENV_VIRTUALENV_DISABLE_PROMPT=1

# Ansible
export ANSIBLE_VAULT_PASSWORD_FILE=~/.secrets/vault_key.py
# AWS
export ANSIBLE_HOSTS=/etc/ansible/ec2.py
export EC2_INI_PATH=/etc/ansible/ec2.ini
if [ -s $HOME/.awsam/bash.rc ]; then
       source $HOME/.awsam/bash.rc
   fi

# Android
export ANDROID_HOME=/Users/danquinn/Library/Android/sdk
export PATH=$PATH:$ANDROID_HOME/platform-tools:$ANDROID_HOME/tools:$ANDROID_HOME/build-tools
# Aliases
#alias ansible-playbook="ansible-playbook -i ~/code/infrastructure/bin/ec2.py"
#sanitized aem example alias:
alias aws_account_name="aem use aws_account_name && souce $HOME/.boto/boto_credentials.sh && export AWS_PROFILE_ZSH='aws_account_name'"
alias py3="pyenv activate py353"
alias py2714="pyenv activate py2714"
alias ans22="pyenv activate ans22"
alias ans23="pyenv activate ans23"
alias ans24="pyenv activate ans24"
alias ruby242="rbenv shell 2.4.2"
alias playbooks="cd ~/code/infrastructure/playbooks"
alias roles="cd ~/code/infrastructure/roles"
alias infra="cd ~/code/infrastructure"
alias code="cd ~/code"
alias weather="curl wttr.in/41.8853162,87.6296955"
