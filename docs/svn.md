SVN 备忘清单
===

本备忘单总结了常用的 [SVN](https://subversion.apache.org/) 命令行指令，以供快速参考。

入门
----

### 基础操作

克隆存储库(代码仓库)

```shell
svn checkout <svn_url>
```

将存储库克隆到指定目录

```shell
svn checkout <svn_url> 指定目录
```

查看代码修改状态

```shell
svn status
```

添加文件

```shell
# 添加单个文件
svn add file

# 添加文件夹
svn add file_folder/
```

提交文件

```shell
svn commit -m "commit message"
```

更新文件

```shell
# 更新整个项目
svn update

# 更新单个文件
svn update file

# 更新单个文件夹
svn update file_folder/
```

### 版本管理

撤销修改

```shell
# 撤销单个文件
svn revert file
```

更新到特定版本

```shell
# 更新到特定版本
svn update -r 1902
```

切换分支

```shell
svn switch <url>
```
