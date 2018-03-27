## Setting up terminal
  sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
 
## To see a better git Log
  git config --global alias.lg "log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit"
  
## Set the Powerline fonts
  https://github.com/powerline/fonts


## POWERLEVEL9K configuration
POWERLEVEL9K_SHORTEN_DIR_LENGTH=2
POWERLEVEL9K_SHORTEN_DELIMITER=""
POWERLEVEL9K_SHORTEN_STRATEGY="truncate_from_right"

alias snl="RAILS_ENV=test bundle exec rspec; lint; [[ -f package.json ]] && yarn lint"
alias aps="COST_ACCOUNTING_SERVICE_URI=http://localhost:3001 OAUTH_DISABLED=true rails s"
alias sps="DB_USERNAME=root DB_PASSWORD=Morita1049_ rails s -p 3001 -s local"
alias ght="git status"
alias rtg="rake translations:generate"
alias gcm="git checkout master"
alias gpu="git pull"
alias gpo="git push origin HEAD"
alias dsps="DB=cost_accounting_service DB_HOST=database.devhealtheintent.net DB_USERNAME=cost_acct_svc DB_PASSWORD=Ya2recret23sazUkus5Ay7B88Ruspeda rails s -p 3001"
test -e "${HOME}/.iterm2_shell_integration.zsh" && source "${HOME}/.iterm2_shell_integration.zsh"
alias japs="COST_ACCOUNTING_SERVICE_URI=http://cost_accounting_service-dj.us.devhealtheintent.net rails s"

## alias for OAUTH
alias auth="java -jar /Users/vr040462/Project/lib/auth-header-1.4.jar -k db2b285e-02e6-43db-b2ae-361aba8da88f -s uxwVsNBEChEh37J1YHSH02duJ19Pq45T -c"
