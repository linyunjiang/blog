---
title: "Mac developer softwares"
date: 2016-02-21
category: tech
tags: [mac, softwares]
author: flowerwrong
---

首先安装`xcode`，建议直接上app store上下载，速度有点慢，耐心等待。
然后安装`command line tools`，运行 `xcode-select --install` 安装即可。

## 免费软件

#### [homebrew](http://brew.sh/): Mac 下超好用的包管理工具

###### 基本用法

```zsh
brew -h
brew search mysql
brew install mysql
```

#### [homebrew cask](http://caskroom.io/): homebrew 扩展

###### 安装

`brew tap caskroom/cask`

###### 基本用法

```zsh
brew search google-chrome
brew cask install google-chrome
```

#### [oh-my-zsh](https://github.com/robbyrussell/oh-my-zsh): 帮助你管理zsh软件的利器
#### iTerm2 + tmux: mac terminal 增强
#### dash: 查看 api 文档的工具, install via app store
#### [atom editor](http://atom.io/)
#### wireshark: 抓包软件

```zsh
brew install wireshark --with-qt
sudo wireshark
```

#### [janus(vim)](https://github.com/carlhuda/janus)
#### google-chrome: install with brew
#### sourcetree: install with brew
#### shadowsocks-libev: install brew

## 开发环境

### nodejs

`brew install nodejs`

### ruby

1. install [rvm](http://rvm.io/)
2. `rvm install ruby-2.3.0`
3. `rvm use ruby-2.3.0 --default`

### java

`brew cask install java`

### database

```zsh
brew install mysql
brew install redis
```

### 开机启动

```zsh
# redis
ln -sfv /usr/local/opt/redis/*.plist ~/Library/LaunchAgents
launchctl load ~/Library/LaunchAgents/homebrew.mxcl.redis.plist

# mysql
ln -sfv /usr/local/opt/mysql/*.plist ~/Library/LaunchAgents
launchctl load ~/Library/LaunchAgents/homebrew.mxcl.mysql.plist
```

## 待续
