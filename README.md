# ENV for ALL Platforms
避免重复折腾，记录一些常用的环境配置。

## MacOS

1. zsh + oh-my-zsh
```bash
brew install zsh
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
# change default shell
chsh -s /bin/zsh
# 设置主题
vim ~/.zshrc
# ZSH_THEME="ys"
```

## Windows

1. Windows Terminal
```bash
# 安装 Windows Terminal
winget install Microsoft.WindowsTerminal -y
```

2. oh-my-posh + posh-git + PSReadLine
```bash
Install-Module oh-my-posh -Scope CurrentUser
Install-Module posh-git -Scope CurrentUser
Install-Module PSReadLine -Scope CurrentUser
# 设置主题
Set-PoshPrompt -Theme ys
```

3. choco
```bash
# 安装 choco
Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
```

## Linux

1. zsh + oh-my-zsh
```bash
sudo apt install zsh
sh -c "$(curl -fsSL https://raw.github.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
# change default shell
chsh -s /bin/zsh
# 设置主题
vim ~/.zshrc
# ZSH_THEME="ys"
```

2. tmux
```bash
sudo apt install tmux
```

## Host

1. ssh
```bash
ssh-keygen -t rsa -b 4096 -C "YOUR_EMAIL"
```
