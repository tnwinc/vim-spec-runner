vim-spec-runner
===============

Vim Commands to execute mocha specs

See it in action: http://www.youtube.com/watch?v=ZOW4V4iRMJc

This vimscript exposes functions to run specs in either named screen sessions or iTerm2, whichever you prefer

If you are using janus, these mappings should probably go in ~/.vimrc.after

Install and configure Bash 4 
----------------------------
```
brew install bash
```

Add /usr/local/bin/bash to /etc/shells file

Make bash4 your default login shell by doing the following

Preferences -> Users and Groups -> right click on your username -> Advanced Options

Mappings for use with iTerm2
----------------------------

```
map <leader>T :call RunAllTestsInITerm()<CR>
map <leader>t :call RunLocalTestsInITerm()<CR>
map <leader>t. :call RunSpecificTestsInITerm()<CR>
map <leader>D :call DebugAllTestsInITerm()<CR>
map <leader>d :call DebugLocalTestsInITerm()<CR>
map <leader>d. :call DebugSpecificTestsInITerm()<CR>
map <leader>tl :call RunLastTestsInITerm()<CR>
```

Mappings for use with Screen
----------------------------

```
map <leader>T :call RunAllTestsInScreen()<CR>
map <leader>t :call RunLocalTestsInScreen()<CR>
map <leader>t. :call RunSpecificTestsInScreen()<CR>
map <leader>D :call DebugAllTestsInScreen()<CR>
map <leader>d :call DebugLocalTestsInScreen()<CR>
map <leader>d. :call DebugSpecificTestsInScreen()<CR>
map <leader>tl :call RunLastTestsInScreen()<CR>
```

