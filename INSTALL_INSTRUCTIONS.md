Install Instructions
====================

1. `/usr/local/bin/zsh`
2. `git clone --recursive https://github.com/iainbeeston/prezto.git "${ZDOTDIR:-$HOME}/.zprezto"`
3. ```sh
     setopt EXTENDED_GLOB
     for rcfile in "${ZDOTDIR:-$HOME}"/.zprezto/runcoms/^README.md(.N); do
       ln -s "$rcfile" "${ZDOTDIR:-$HOME}/.${rcfile:t}"
     done
   ```
4. `git clone --recurse-submodules https://github.com/belak/prezto-contrib "${ZPREZTODIR}/contrib"`
5. `sudo echo "/usr/local/bin/zsh" > /etc/shells`
6. `chsh -s /usr/local/bin/zsh`