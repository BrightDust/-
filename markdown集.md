# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题（支持到六级）
**加粗**

*斜体*

***加粗斜体***

~~删除线~~（没有实现）

原因：前端预览是js渲染的，后端输出php处理的，两者的markdown语法有差异
~~来做删除线被认为是不规范的markdown语法，js渲染那边会去掉。

解决方法：<del>我是被删除的</del>

> 引用
>> 引用
>>>引用的嵌套

分割线
***
---

图片
![图片alt内容的解释](图片地址"图片标题")

超链接
[超链接名](超链接地址"超链接标题·可加可不加")

[百度](http://baidu.com)

列表无序

- 列表内容（中间要有空格）
+ 列表内容
* 列表内容

有序列表（数字加点）

1. 列表内容
2. 列表内容
3. 列表内容

列表嵌套

上一级和下一级之间敲三个空格(未实现)

##表格

姓名|技能|排行
--|:--:|--:
刘备|哭|大哥
关羽|打|二哥
张飞|骂|三弟

##代码
(` 在键盘左上角，1旁边)

`代码内容`

```
   代码
```

###示例

`create database hero`

```
   function fun(){
      ech0 "这是一句非常厉害的代码"；
   }
```

##流程图

```flow

st=>start: 开始

op=>operation: My Operation

cond=>condition: Yes or No?

e=>end

st->op->cond

cond(yes)->e

cond(no)->op

```

```flow
st=>start: Start|past:>http://www.google.com[blank]
e=>end: End:>http://www.google.com
op1=>operation: My Operation|past
op2=>operation: Stuff|current
sub1=>subroutine: My Subroutine|invalid
cond=>condition: Yes
or No?|approved:>http://www.google.com
c2=>condition: Good idea|rejected
io=>inputoutput: catch something…|request

st->op1(right)->cond
cond(yes, right)->c2
cond(no)->sub1(left)->op1
c2(yes)->io->e
c2(no)->op2->e
```