---
tags: ['版本控制', 'Git-2.39.1']

---

# Git教程

## Git软件信息查看

- 查看git软件版本: `git --version`
- 查看git帮助文档: `git --help`

## Git默认配置
一般来说，Git运行时，外观和行为的默认配置存储在如下三个文件:

- `/etc/gitconfig`文件: 系统级的git配置;
- `~/.gitconfig`文件: 用户级的git配置;
- 项目目录下的`.git/config`文件: 项目级的git配置。

配置文件的语法类似与toml语法。对git的配置的创建和更改具有两个方式:

- 使用编辑器手动创建和修改;
- 使用`git config`命令创建和修改。此种方式适合少量参数配置情形以及不方便启动编辑器的情形。


!!! note 
	1. 配置文件并没在Git安装后自动创建, 前两个仅仅在使用`git config`语句配置信息后生成，一般使用`git config --global user.name="your_name"`创建用户配置文件并配置用户名，利用root全县并更改`--global`为`--system`对应系统级配置; 第三个在git项目创建时生成。
	2. 运行Git时，配置信息会自动覆盖上一级别的配置，即当三个文件中相同配置参数具有不同的值，优先使用下一级别文件中的值。如在`~/.gitconfig`中的`user.name = kyrie_user`, 而项目目录下的`.git/config`文件中的`user.name = kyrie_project`时，使用git提交文件将使用`kyrie_project`作为用户名。	
!!! important
	建议在Git首次安装后，马上创建和修改用户级的配置文件（系统级配置尽量不要动），主要Git文件权限、外观和默认编辑器等; 当创建一个git项目时，对更改项目级的配置，主要是git用户帐号相关信息。

### 常用配置参数

### 账户


#### 文件权限

#### 外观


#### 编辑工具


####






## Git

- 初始化仓库: `git init`

- 创建新分支: 
