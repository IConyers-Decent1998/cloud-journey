Path is a enviroment variable that tells your system where to look for programs. Path in simple terms is a shortcut without having to type out all files to where you wanna go.
Programs are found automatically but sometimes path won't find them, then you have to add the sequence of file to get where you want to manually and after that it will be saved.
My example of me doing it (with help): 

Isaiah@DESKTOP-066RCFJ MINGW64 ~
$ echo $PATH
/c/Users/Isaiah/bin:/mingw64/bin:/usr/local/bin:/usr/bin:/bin:/mingw64/bin:/usr/bin:/c/Users/Isaiah/bin:/c/WINDOWS/system32:/c/WINDOWS:/c/WINDOWS/System32/Wbem:/c/WINDOWS/System32/WindowsPowerShell/v1.0:/c/WINDOWS/System32/OpenSSH:/c/Program Files (x86)/NVIDIA Corporation/PhysX/Common:/c/Program Files/NVIDIA Corporation/NVIDIA NvDLISR:/cmd:/c/Users/Isaiah/AppData/Local/Microsoft/WindowsApps:/c/Users/Isaiah/AppData/Local/Programs/Microsoft VS Code/bin:/usr/bin/vendor_perl:/usr/bin/core_perl

Isaiah@DESKTOP-066RCFJ MINGW64 ~
$ mkdir ~/my-scripts

Isaiah@DESKTOP-066RCFJ MINGW64 ~
$ cd ~/my-scripts

Isaiah@DESKTOP-066RCFJ MINGW64 ~/my-scripts
$ touchtest.sh
bash: touchtest.sh: command not found

Isaiah@DESKTOP-066RCFJ MINGW64 ~/my-scripts
$ touch test.sh

Isaiah@DESKTOP-066RCFJ MINGW64 ~/my-scripts
$ echo "echo Hello Path" > test.sh

Isaiah@DESKTOP-066RCFJ MINGW64 ~/my-scripts
$ chmod +x test.sh

Isaiah@DESKTOP-066RCFJ MINGW64 ~/my-scripts
$ export PATH=$PATH:~/my-scripts

Isaiah@DESKTOP-066RCFJ MINGW64 ~/my-scripts
$ test.sh
Hello Path

Isaiah@DESKTOP-066RCFJ MINGW64 ~/my-scripts
$

