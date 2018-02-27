# MarkdownNote
## 1.标题 
# head1
## head2
### head3
#### head4
##### head5
###### head6
####### head7 //wrong

## 2.引用
tab 引用换行
> hello world!

> hello world!  
> hello world!  
> hello world!  

引用嵌套
>a
>>a
>>>a

## 3.行内标记
out `hellow world` out

## 4.代码块
使用```生成代码块
```
<div>
    <div></div>
    <div></div>
    <div></div>
    <div></div>
</div>
```

```javascript
var num = 0;
for (var i = 0; i < 5; i++) {
    num+=i;
}
console.log(num);
```

## 4.链接
行内式链接，只要在方块括号后面紧接着圆括号并插入网址链接即可，如果你还想要加上链接title 文字，只要在网址后面，用双引号把 title 文字包起来即可  

This is [an example](http://example.com/ "Title") inline link.  
[This link](http://example.net/) has no title attribute.    

参考式的链接是在链接文字的括号后面再接上另一个方括号，而在第二个方括号里面要填入用以辨识链接的标记:  
This is [an example][id] reference-style link.  

[id]: http://example.com/  "Optional Title Here"

链接内容定义的形式为：

* 方括号（前面可以选择性地加上至多三个空格来缩进），里面输入链接文字
* 接着一个冒号
* 接着一个以上的空格或制表符
* 接着链接的网址
* 选择性地接着 title 内容，可以用单引号、双引号或是括弧包着
* 下面这三种链接的定义都是相同：
```
[foo]: http://example.com/  "Optional Title Here"
[foo]: http://example.com/  'Optional Title Here'
[foo]: http://example.com/  (Optional Title Here)
```

## 5.表
有序
1. one
2. two
3. three

无序
* one
* two 
* three

序表嵌套
1. one 
    1. one-1
    2. one-2
        1. one-2.1
2. two
    * two-1
    * two-2

序表嵌套代码块
* one

    ```var a = 10; ```
* two

## 6.任务列表

- [x] 1
- [ ] 2
- [ ] 3

## 7.表格
|    a    |       b       |      c     |
|:-------:|:------------- | ----------:|
|   居中  |     左对齐    |   右对齐   |
|=========|===============|============|

## 8.语义标记
*aaa*

_aaa_ 

**aaa**

__aaa__

***aaa***

~~aaa~~

## 9.语义标签

<i>aaa</i>

<b>aaa</b>

<em>aaa</em>

Z<sup>a</sup>

Z<sub>a</sub>

<kbd>Ctrl</kbd>

## 10.公式

1个$左对齐，2个居中

$$ x \href{why-equal.html}{=} y^2 + 1 $$

$ x = {-b \pm \sqrt{b^2-4ac} \over 2a}. $

## 11.分隔符
***
---

## 12.脚注

Markdown[^1]    

[^1]: Markdown是一种纯文本标记语言        // 在文章最后面显示脚注

## 13.自动邮箱链接
<xxx@outlook.com>

## 14.流程图
```flow                     // 流程
st=>start: 开始|past:> http://www.baidu.com // 开始
e=>end: 结束              // 结束
c1=>condition: 条件1:>http://www.baidu.com[_parent]   // 判断条件
c2=>condition: 条件2      // 判断条件
c3=>condition: 条件3      // 判断条件
io=>inputoutput: 输出     // 输出
//----------------以上为定义参数-------------------------

//----------------以下为连接参数-------------------------
// 开始->判断条件1为no->判断条件2为no->判断条件3为no->输出->结束
st->c1(yes,right)->c2(yes,right)->c3(yes,right)->io->e
c1(no)->e                   // 条件1不满足->结束
c2(no)->e                   // 条件2不满足->结束
c3(no)->e                   // 条件3不满足->结束
```
