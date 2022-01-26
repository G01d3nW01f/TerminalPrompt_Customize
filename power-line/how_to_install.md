   Install
    
    ```pip install --user powerline-shell```
    
   Uninstall 
    
    ```pip uninstall --user powerline-shell```
    
   Config in bash to "~/.bashrc"
   
   ```
   function _update_ps1() {
    PS1="$(~/.local/bin/powerline-shell $?)"
  }
      
  if [ "$TERM" != "linux" ]; then
      PROMPT_COMMAND="_update_ps1; $PROMPT_COMMAND"
  fi
  ```
