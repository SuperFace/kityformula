kityformula
===========

WEB mathematical formulas projects

# 子项目：
```
editor KityFormula Editor 基于 SVG 的公式编辑器
parser Kity Formula Parser
render Kity Formula Render（KFR） 是一个基于SVG的公式渲染引擎，用以降低在web上呈现数学公式的复杂度。KFR是一个纯浏览器端解决方案，以**完全脱离服务器**的方式渲染公式，最终产生的公式可以是栅格化的图片，也可以是矢量化的图形。
```

# submodule:
```
添加
为当前工程添加submodule，命令如下：

git submodule add 仓库地址 路径
其中，仓库地址是指子模块仓库地址，路径指将子模块放置在当前工程下的路径。 
注意：路径不能以 / 结尾（会造成修改不生效）、不能是现有工程已有的目录（不能順利 Clone）

命令执行完成，会在当前工程根路径下生成一个名为“.gitmodules”的文件，其中记录了子模块的信息。添加完成以后，再将子模块所在的文件夹添加到工程中即可。

删除
submodule的删除稍微麻烦点：首先，要在“.gitmodules”文件中删除相应配置信息。然后，执行“git rm –cached ”命令将子模块所在的文件从git中删除。

下载的工程带有submodule
当使用git clone下来的工程中带有submodule时，初始的时候，submodule的内容并不会自动下载下来的，此时，只需执行如下命令：

git submodule update --init --recursive
```
