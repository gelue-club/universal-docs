# 准备开发环境

## 目录

- [推荐使用 Linux/Unix 系统](#推荐使用-linuxunix-系统)
- [在全网环境（借助 VPN）下工作](#在全网环境借助-vpn下工作)
- [使用 Chrome 浏览器](#使用-chrome-浏览器)
- [使用 Git 协作开发](#使用-git-协作开发)
  - [安装软件](#安装软件)
  - [征服 Git](#征服-git)
- [使用 Git Flow 工作流](#使用-git-flow-工作流)
- [借助 ZSH 加强你的命令行界面](#借助-zsh-加强你的命令行界面)
  - [安装 OH-MY-ZSH](#安装-oh-my-zsh)
  - [更新 OH-MY-ZSH 的配置](#更新-oh-my-zsh-的配置)
  - [Linux 提示](#linux-提示)
- [通过 NVM 管理不同版本的 Node.js](#通过-nvm-管理不同版本的-nodejs)
  - [安装 NVM](#安装-nvm)
- [统一使用 Atom/VSCode 编辑器](#统一使用-atomvscode-编辑器)

## 推荐使用 Linux/Unix 系统

系统支持，

- Linux，如：Ubuntu, CentOS, 等等
- OS X

上述并非表明不支持其它系统，只不过我们专注于在上述系统中完成工作。

## 在全网环境（借助 VPN）下工作

虽然有淘宝 NPM、GEM 等国内镜像的支持，但是不可排除部分库自身会从国外诸如亚马逊服务器上下载依赖的情况，比如：Phantom.js，为了避免相关情况影响到实际生产效率，推荐在全网环境下进行开发活动，一次性解决所有潜在的库下载问题等。

## 使用 Chrome 浏览器

Chrome 浏览器的开发者工具、插件生态、性能等无与伦比，推荐参阅 [Chromium Blog](https://blog.chromium.org/)、[BATTLE OF THE BROWSERS: EDGE VS. CHROME VS. FIREFOX VS. OPERA VS. VIVALDI](https://www.digitaltrends.com/computing/best-browser-internet-explorer-vs-chrome-vs-firefox-vs-safari-vs-edge/) 以了解更多。

## 使用 Git 协作开发

### 安装软件

（使用 Linux(Ubuntu, etc) 或者 Unix(Mac OS X) 系统的筒子飘过这一段）如果你使用 Windows 7+ 系统，需要 **依序 全局安装** 下述软件，否则忽略，
- [Chocolatey](https://chocolatey.org/install) ( 参阅 [`Windows 系统的包管理器 Chocolatey`](http://www.tuicool.com/articles/QV7VNrR) 以安装 )
- [Wget ( 管理员权限下运行 Power Shell 命令行界面输入 `choco install wget` 以安装 )](https://www.gnu.org/software/wget/)

无论你使用的是 Linux(Ubuntu, etc)、Unix(Mac OS X) 抑或 Windows 系统，**依序 全局安装** 下述软件，

- Git ( [win 2.11.1 / osx 2.11.1 / Linux](https://git-scm.com/) )
- [GitFlow ( 使用 Wget 的方式安装 )](https://github.com/nvie/gitflow/wiki/Windows#cygwin)
- [GitKraken ( Git 图形界面 )](https://www.gitkraken.com/)
- [GitDeep](http://www.syntevo.com/deepgit/)

> 依序完成上述预估耗时 15 分钟。

### 征服 Git

通过 [`Try Git`](https://try.github.io/levels/1/challenges/1?__utma=1.580116084.1384070580.1384070580.1384070580.1&__utmb=1.14.10.1384070580&__utmc=1&__utmk=61742508&__utmv=-&__utmx=-&__utmz=1.1384070580.1.1.utmcsr%3D%28direct%29%7Cutmccn%3D%28direct%29%7Cutmcmd%3D%28none%29) 平台快速学习 Git 常用指令，尽管后期是通过 GitKraken 的图形界面操作，但是对常用 Git 指令的学习可以帮助理解 Git 及 [`git-flow`](https://github.com/nvie/gitflow) 工作流。( PS: 开发过程中你可以使用命令亦或是图形界面执行 Git 操作，哪个有快感用哪个 )

[GitKraken ( Git 图形界面 )](https://www.gitkraken.com/) 的使用参见它自己的[文档](https://support.gitkraken.com/)，易上手。

开展协作前，充分阅读、理解 [`git-flow`](https://github.com/nvie/gitflow) 工作流，可综合 [`Git Flow是什么?`](https://segmentfault.com/a/1190000006194051) & [`企业级开发：Gitflow Workflow工作流`](http://www.jianshu.com/p/104fa8b15d1e) 来理解。

熟悉 Github 的方方面面对基于 Git 的协作也会有各种便利之处。

> 在 Windwos 下开发的筒子们，如果你的 Git Bash 无法使用 Git Flow，就通过 Power Shell 进行操作。

## 使用 Git Flow 工作流

参阅 [A successful Git branching model](http://nvie.com/posts/a-successful-git-branching-model/) 以深入了解什么是 `Git Flow`，参阅 [Installing git-flow](https://github.com/nvie/gitflow/wiki/Installation) 安装。

## 借助 ZSH 加强你的命令行界面

### 安装 OH-MY-ZSH

安装 [OH-MY-ZSH](http://ohmyz.sh/) 前，先确保成功安装了 [ZSH](https://github.com/robbyrussell/oh-my-zsh/wiki/Installing-ZSH)。

接着，执行下述指令之一以完成 [OH-MY-ZSH](http://ohmyz.sh/) 的安装，

```shell
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

或者，

```shell
sh -c "$(wget https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)"
```

如果想要了解更多安装方面，查阅官方 [快速开始](https://github.com/robbyrussell/oh-my-zsh#getting-started) 文档。

### 更新 OH-MY-ZSH 的配置

***这份配置文件（.zshrc）在当前系统用户根目录下***，Unix(Mac OS X) 下直接运行下述指令即可在 [Vim](https://vim.sourceforge.io/) 模式下编辑该配置文件，

```shell
vi ~/.zshrc
```

如果是 Linux(Ubuntu) 桌面系统的话，推荐用 **文本编辑器** 编辑。

默认情况下，配置文件（.zshrc）中会包含 `plugins=(git)` 这样的内容，可以通过全文搜索的办法定位到，替换成下述内容即可，

```
plugins=(git nvm rvm node yarn gulp grunt autojump aws bower python branch copydir copyfile cp docker-compose docker emoji-clock emoji encode64 gem git-extras git-flow-avh git-flow git-hubflow git-prompt git-remote-branch gitfast github gitignore history history-substring-search meteor npm pass pip sudo sublime svn vi-mode zsh_reload ubuntu)
```

> 依序完成上述预估耗时 5 分钟。

### Linux 提示

- 配置命令行界面 `文件首选项` 时选中 `运行自定义命令而不是 Shell` 选项，并且在自定义命令域中输入 `zsh` 指令，如果你没有自定义 `zsh` 初始化指令化名的情况下。

> 依序完成上述预估耗时 5 分钟。

## 通过 NVM 管理不同版本的 Node.js

### 安装 NVM

运行下述指令，

```shell
curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.2/install.sh | bash
```

如果想要了解更多，可以访问 [NVM 在 Github 上的项目](https://github.com/creationix/nvm)。

## 统一使用 Atom/VSCode 编辑器

**实时构建** 的过程中不包含代码的各种检测可以带来更高的 **实时构建** 效率，基于这样的考虑，我们默认将诸如书写、类型、语法检测等任务交给编辑器以提升实时构建的效率等，也正是如此，我们需要统一编辑器的使用约定，

:traffic_light: **注重编辑器的提示界面，推荐使用 [Atom](https://atom.io/)**，去 [官网](https://atom.io/) 下载安装包以安装 Atom 编辑器，

> Ubuntu 筒子们可参阅 [How to install Atom editor in Ubuntu 14.04](https://codeforgeek.com/2014/09/install-atom-editor-ubuntu-14-04/) 或 [Install Atom Text Editor in Ubuntu 16.04 (both 32&64bit)](http://tipsonubuntu.com/2016/08/05/install-atom-text-editor-ubuntu-16-04/) 这 2 篇文章中任意一篇通过命令行界面安装 Atom 编辑器。

安装 Atom 插件，

```shell
sh ./tool/apm.global.install.sh   # 如果使用的是 OS X 系统
```

另外，可以了解下面列出来的插件，可以加强你的 Atom 编辑器及使用体验（但是也可能会让编辑器的效率降低），

- [nuclide](https://atom.io/packages/nuclide)
- [nuclide-format-js](https://atom.io/packages/nuclide-format-js)
- [emmet](https://atom.io/packages/emmet)
- [editor-stats](https://atom.io/packages/editor-stats)
- [custom-title](https://atom.io/packages/custom-title)
- [activate-power-mode](https://atom.io/packages/activate-power-mode)
- [auto-update-packages](https://atom.io/packages/auto-update-packages)
- [haskell-grammar](https://atom.io/packages/haskell-grammar)
- [language-fish-shell](https://atom.io/packages/language-fish-shell)
- [language-gradle](https://atom.io/packages/language-gradle)
- [language-lua](https://atom.io/packages/language-lua)
- [language-ocaml](https://atom.io/packages/language-ocaml)
- [language-thrift](https://atom.io/packages/language-thrift)
- [MagicPython](https://atom.io/packages/MagicPython)
- [pretty-json](https://atom.io/packages/pretty-json)
- [travis-ci-status](https://atom.io/packages/travis-ci-status)
- [sync-settings](https://atom.io/packages/sync-settings)
- [remote-edit](https://atom.io/packages/remote-edit)
- [linter-tslint](https://atom.io/packages/linter-tslint)
- [language-swift](https://atom.io/packages/language-swift)
- [hey-pane](https://atom.io/packages/hey-pane)
- [set-syntax](https://atom.io/packages/set-syntax)
- [an-old-hope-syntax](https://atom.io/packages/an-old-hope-syntax)

结合上面插件的 Atom 详细配置参见这个 [Gist](https://gist.github.com/iTonyYo/759c04a87501425a6861d6f19b4a2202)，如何自定义 Atom 参见官方的 [介绍](http://flight-manual.atom.io/using-atom/sections/basic-customization/)。

:traffic_light: **更在乎编辑器的性能，推荐使用 [Visual Studio Code](https://code.visualstudio.com/)**，去 [官网](https://code.visualstudio.com/Download) 下载安装包以安装 Visual Studio Code 编辑器，

安装 Visual Studio Code 插件，

> 提示：下述将 `Visual Studio Code 编辑器` 简述为 `VS Code`。

- EditorConfig for Visual Studio Code
- VS Code ESLint extension
- vscode-jest
- JSCS Linting
- Project Manager
- scss-lint

另外，可以了解下面列出来的插件，可以加强你的 VS Code 编辑器及使用体验，

- seti-icons
- vscode-icons

VS Code 的详细配置已经可视化在 `.vscode` 目录下，如果想要了解如何 [自定义 VS Code](https://code.visualstudio.com/docs/introvideos/configure)，参见官方 [介绍](https://code.visualstudio.com/docs/introvideos/configure)。