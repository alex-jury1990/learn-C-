# learn-C-
_anything_


#git colours
parse_git_branch() {
     git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/ (\1)/'
}
export PS1='\u \[\e[95m\]\W \[\e[32m\]$(parse_git_branch)\[\e[00m\]$ '
