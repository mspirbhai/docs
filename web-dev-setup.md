https://fireship.io/lessons/windows-10-for-web-dev/

```
sudo apt install zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

sudo apt-get install fonts-powerline
code ~/.zshrc # to customize it
```
Prefered theme is: ZSH_THEME="philips"

As a web developer you need Node.js. You can manage multiple versions with NVM.
```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash
```
plugins=(git nvm)
```
nvm install --lts

node -v
npm -v

nvm alias default node
```

Cache Remote Login Credentials
```
git config --global user.name "Jeff Delaney"
git config --global user.email "hello@fireship.io"
git config --global credential.helper cache --timeout=3600
```

