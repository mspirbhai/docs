1. install git for windows

2. install git for WSL
    
3. Set the global config for using GCM (Windows)
    `git config --global credential.helper "/mnt/c/Program\ Files/Git/mingw64/bin/git-credential-manager.exe"`

4. Set the global username
    `git config --global user.name "User Name"`

5. Set the global email
    `git config --global user.email "User@Email"`

6. (Opt) Set the default head
    `git branch --set-upstream-to=origin/main main`
