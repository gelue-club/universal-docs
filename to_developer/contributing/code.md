草稿参阅
https://zh-hans.reactjs.org/docs/codebase-overview.html



# 贡献代码

如果你想要做出第一次贡献，只需按照以下简单步骤操作即可。我们答应你，这将很好玩 :)

<img align="right" width="300" src="https://raw.githubusercontent.com/firstcontributions/first-contributions/master/assets/fork.png" alt="fork this repository" />

如果你的电脑上尚未安装 git, 请按照这个[ 安装指引 ](https://help.github.com/articles/set-up-git/)进行安装。

### Fork（复制）本代码仓库

点击图示中的按钮去 Fork 这个代码仓库。
这个操作会将代码仓库复制到你的账户名下。

### Clone（克隆）代码仓库

<img align="right" width="300" src="https://raw.githubusercontent.com/firstcontributions/first-contributions/master/assets/clone.png" alt="clone this repository" />

接下来，将复制后的代码仓库克隆到你的电脑上。点击图示中的绿色按钮，接着点击复制到剪切板按钮（将代码仓库地址复制下来）

随后打开命令行窗口，敲入如下 git 命令：

```
git clone "刚才复制的 url 链接"
```
"刚才复制的 url 链接"（去掉双引号）就是复制到你账户名下的代码仓库地址。获取这链接地址的方法请见上一步。

<img align="right" width="300" src="https://raw.githubusercontent.com/firstcontributions/first-contributions/master/assets/copy-to-clipboard.png" alt="copy URL to clipboard" />

譬如：
```
git clone https://github.com/你的 Github 用户名/first-contributions.git
```

'你的 Github 用户名' 指的就是你的 Github 用户名。这一步，你将复制到你账户名下的 first-contributions 这个代码仓库克隆到本地电脑上。

### 新建一个分支

下面的命令能在命令行窗口中，把目录切换到 first-contributions
```
cd first-contributions
```

接下来使用 `git checkout` 命令新建一个代码分支
```
git checkout -b <新分支的名称>
```

譬如：
```
git checkout -b add-myname
```

(新分支的名称不一定需要有 *add*。然而，在新分支的名称加入 *add* 是一件合理的事情，因为这个分支的目的是将你的名字添加到列表中。更详细的命名风格约定，参见 [git.md][git.md])

### 对代码进行修改，而後 Commit (提交) 修改

打开 `Contributors.md` 这个文件，更新文件内容，将你的名字加上去，保存修改。`git status` 这命令会列出被改动的文件。接着 `git add` 这命令则可以添加你的改动，就像如下这条命令。

<img align="right" width="450" src="https://raw.githubusercontent.com/firstcontributions/first-contributions/master/assets/git-status.png" alt="git status" />

```
git add Contributors.md
```

现在就可以使用 `git commit` 命令 commit 你的修改了。
```
git commit -m "Add <你的名字> to Contributors list"
```
将 `<你的名字>` 替换为你的名字

### 将改动 Push（发布）到 GitHub

使用 `git push` 命令发布代码
```
git push origin <分支的名称>
```
将 `<分支的名称>` 替换为之前新建的分支名称。

### 提出 Pull Request 将你的修改供他人审阅

前往 Github 你的代码仓库，你会看到一个 `Compare & pull request` 的按钮。点击该按钮。

<img style="float: right;" src="https://raw.githubusercontent.com/firstcontributions/first-contributions/master/assets/compare-and-pull.png" alt="create a pull request" />

接着再点击 `Create pull request` 按钮，正式提交 pull request。

<img style="float: right;" src="https://raw.githubusercontent.com/firstcontributions/first-contributions/master/assets/submit-pull-request.png" alt="submit pull request" />

不久之后，我便会把你所有的变化合并到这个项目的主分支。更改合并后，你会收到电子邮件通知。



[git.md]: #