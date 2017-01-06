# Diary_January
## 2017.01.06 【代码自动格式化工具-插件】

这里说明的是：sublime text3 的 插件的运用

首先这里有一个自动缩进/再次缩进（reindent），实际运用效果并不是很好，用于缩进可以，但是用于展开HTML文件的标签，实在够呛

经过测试有两个插件还是很好用的，第一个是CSS Format 第二个是 JSFormat，这两个都挺好用的

【1】安装插件的方法

1.首先你要安装了package control在你的SublimeText中

2、通过快捷键组合ctrl+shift+P唤出命令面板

3、在面板中输入“install package”后回车

4、接着输入“format”（即格式化的意思），在弹出的列表中找到对应你所想要进行格式化操作的语言


【2】应该如何对该格式化代码功能进行快捷键组合的设置呢？

1、首先通过以下路径打开用户按键绑定文件：

Preferences → Key Bindings – User

2、然后在其中添加以下代码（如果你有需要的话，其中的快捷键组合是可以自己定义的）：

{"keys": ["ctrl+shift+r"], "command": "reindent" , "args": {"single_line": false}}

在这儿请注意每组快捷键组合包含着一个中括号里面，通过大括号定义一组快捷键，然后通过英文逗号进行分隔

