# Diary_January
## 2017.01.06 
## 【代码自动格式化工具-插件】

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

## 【JS截取字符串常用方法】
### 函数：split() 

功能：使用一个指定的分隔符把一个字符串分割存储到数组 

例子： 

str=”jpg|bmp|gif|ico|png”; 

arr=theString.split(”|”); 

//arr是一个包含字符值”jpg”、”bmp”、”gif”、”ico”和”png”的数组 

### 函数：Join() 

功能：使用您选择的分隔符将一个数组合并为一个字符串 

例子： 

var myList=new Array(”jpg”,”bmp”,”gif”,”ico”,”png”); 

var portableList=myList.join(”|”); 

//结果是jpg|bmp|gif|ico|png 

### 函数：substring() 

功能：字符串截取，比如想从"MinidxSearchEngine”中得到"Minidx”就要用到substring(0,6) 

### 函数：indexOf() 
功能：返回字符串中匹配子串的第一个字符的下标 

var myString=”JavaScript”; 

var w=myString.indexOf(”v”);w will be 2 

var x=myString.indexOf(”S”);x will be 4 

var y=myString.indexOf(”Script”);y will also be 4 

var z=myString.indexOf(”key”);z will be -1  //没有找到的就返回-1

### 详解substring 方法 

*定义和用法 *

substring 方法用于提取字符串中介于两个指定下标之间的字符。 

* 语法

stringObject.substring(start,stop) 

* 参数 描述

start 必需。一个非负的整数，规定要提取的子串的第一个字符在 stringObject 中的位置。 

stop 可选。一个非负的整数，比要提取的子串的最后一个字符在 stringObject 中的位置多 1。如果省略该参数，那么返回的子串会一直到字符串的结尾。 

* 返回值 

一个新的字符串，该字符串值包含 stringObject 的一个子字符串，其内容是从 start 处到 stop-1 处的所有字符，其长度为 stop 减 start。 

* 说明 
substring 方法返回的子串包括 start 处的字符，但不包括 end 处的字符。 

如果 start 与 end 相等，那么该方法返回的就是一个空串（即长度为 0 的字符串）。 
 
如果 start 比 end 大，那么该方法在提取子串之前会先交换这两个参数。 

如果 start 或 end 为负数，那么它将被替换为 0。 

### 详解substr 方法 

* 定义和用法 

substr 方法用于返回一个从指定位置开始的指定长度的子字符串。 

* 语法 

stringObject.substr(start [, length ]) 

* 参数 描述 

start 必需。所需的子字符串的起始位置。字符串中的第一个字符的索引为 0。 

length 可选。在返回的子字符串中应包括的字符个数。 

* 说明 

如果 length 为 0 或负数，将返回一个空字符串。 

如果没有指定该参数，则子字符串将延续到stringObject的最后。 

## 2017.01.09 

## 【JS取float型小数点后两位数的方法】

#### 四舍五入

var num =2.446242342;

num = num.toFixed(2); // 输出结果为 2.45

#### 不四舍五入

**第一种**,先把小数变成整数：(Math.floor)就是求一个最接近它的整数

Math.floor(15.7784514000 * 100) / 100  

// 输出结果为 15.77

**第二种**,正则表达式

**取整的方法**

1.丢弃小数部分,保留整数部分 parseInt(5/2)

2.向上取整,有小数就整数部分加1  Math.ceil(5/2)

3.四舍五入 Math.round(5/2)

4.向下取整 Math.floor(5/2)

## 【认识和入门Markdown】
> http://sspai.com/25137
