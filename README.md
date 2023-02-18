# my_personal_aliases

#### This alias compiles C files in the current directory with warnings enabled using --Wall and prompts the user to run the compiled program. If the user inputs "y" or "Y", the program is executed via ./app.

```
alias gccall='gcc -o app *.c --Wall && read -p "Compile successful. Run program? [y/n] " choice && [ "$choice" == "y" -o "$choice" == "Y" ] && ./app'
```
-----

