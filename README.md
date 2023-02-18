# my_personal_aliases

## Notice

Most things where were generated with the help of chatGPT

------

## How to use ubuntu aliases in windows?

Aliases in Ubuntu are implemented using the Bash shell, which is the default shell in Ubuntu. 

Windows, on the other hand, uses the Command Prompt or PowerShell as the default shell, which does not natively support Bash aliases. 

However, you can use the Windows Subsystem for Linux (WSL) to run Ubuntu on Windows and take advantage of its Bash shell and aliases.

### Here are the steps to set up and use Ubuntu aliases in Windows using WSL:

##### 1. Install WSL on your Windows machine. You can follow the official Microsoft documentation to install WSL: https://docs.microsoft.com/en-us/windows/wsl/install-win10

##### 2. Once you have installed WSL, you can install Ubuntu from the Microsoft Store or download and install it manually. Make sure to choose the version of Ubuntu that you prefer.

##### 3. After installing Ubuntu, launch the Ubuntu terminal from the Start menu or from the Microsoft Store.

##### 4. Once you are in the Ubuntu terminal, you can create and modify aliases in the same way as you would on a native Ubuntu installation. 


------

#### This alias compiles C files in the current directory with warnings enabled using --Wall and prompts the user to run the compiled program. If the user inputs "y" or "Y", the program is executed via ./app.

```
alias gccall='gcc -o app *.c -Wall && read -p "Compile successful. Run program? [y/n] " choice && [ "$choice" == "y" -o "$choice" == "Y" ] && ./app'
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
alias create_env_with='pip install --upgrade --user pip && pip install --upgrade --user virtualenv && virtualenv project_virtual_env && source project_virtual_env/bin/activate && read -p "Enter the package name to install: " pkgname && pip install $pkgname'
```

-----

