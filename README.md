A Powerline style prompt for your shell
=======================================

Cloned from https://github.com/milkbikis/powerline-shell:

### Bash:
Add the following to your `.bashrc` (or `.profile` on Mac):

        function _update_ps1() {
           PS1="$(~/powerline-shell.py $? 2> /dev/null)"
        }

        if [ "$TERM" != "linux" ]; then
            PROMPT_COMMAND="_update_ps1; $PROMPT_COMMAND"
        fi

