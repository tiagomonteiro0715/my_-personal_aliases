# my_personal_aliases

#### This alias compiles C files in the current directory with warnings enabled using --Wall and prompts the user to run the compiled program. If the user inputs "y" or "Y", the program is executed via ./app.

```
alias gccall='gcc -o app *.c --Wall && read -p "Compile successful. Run program? [y/n] " choice && [ "$choice" == "y" -o "$choice" == "Y" ] && ./app'
```
-----

#### This alias performs the following actions in order:
##### 1. Upgrades pip to the latest version.
##### 2. Installs virtualenv via pip.
##### 3. Creates a new virtual environment called project_virtual_env.
##### 4. Activates the virtual environment.
##### 5. Prompts the user to enter the name of a package to install.
##### 6. Installs the specified package via pip.

```
alias create_env_with ='pip install --upgrade --user pip && pip install --upgrade --user virtualenv && virtualenv project_virtual_env && source project_virtual_env/bin/activate && read -p "Enter the package name to install: " pkgname && pip install $pkgname'
```

-----

