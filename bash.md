```bash
export CLICOLOR=1
export LSCOLORS=dxgxxxxxFxxxxxxxxxxxex

# ALIASES
alias l='ls -lh'
alias ll='ls -lha'
alias lh='ls -lh'

# current timestamp
alias ts='date +%s'

# ports
alias ports='lsof -i -P'

# colorize terminal
function color_my_prompt {
  local __user="\[\033[01;32m\]\u"
  local __user_and_host="\[\033[01;32m\]\u@\h"
  local __cur_location="\[\033[01;34m\]\w"
  local __cur_dir="\[\033[1;33m\]\W"
  local __git_branch_color="\[\033[31m\]"
  local __git_branch=' `git branch 2> /dev/null | sed -e "/^[^*]/d" -e "s/* \(.*\)/(\1)/"`'
  local __prompt_tail="\[\033[35m\]$"
  local __last_color="\[\033[00m\]"
  export PS1="$__user $__cur_dir$__git_branch_color$__git_branch$__prompt_tail$__last_color "
}
color_my_prompt

```
