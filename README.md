# **Markdown** `github`
## Syntax guide `语法指南`

### Headers `标题`
使用方法：在文本前面加上`#`号，`#`与文本之间隔一个空格，即可显示为标题效果
```
# This is an <h1> tag
## This is an <h2> tag
###### This is an <h6> tag
```
> 效果如下：  
# 标题一
## 标题二
###### 标题六   

---

### Emphasis `文本：加粗，斜体`
```
*This text will be italic*
_This will also be italic_

**This text will be bold**
__This will also be bold__

_You **can** combine them_
```
> 效果如下：  
 `tips: 如果要换行，只需在需要换行的文本后面加上两个空格即可。`  

*This text will be italic*  
_This will also be italic_  
**This text will be bold**  
__This will also be bold__  
_You **can** combine them_  

----
### Lists `列表`

#### Unordered `无序列表`
```
* Item 1
* Item 2
  * Item 2a
  * Item 2b
```
> 效果如下：  

* Item 1
* Item 2
  * Item 2a
  * Item 2b

#### Ordered `有序列表`
```
1. Item 1
1. Item 2
1. Item 3
   1. Item 3a
   1. Item 3b
```
> 效果如下：  

1. Item 1
1. Item 2
1. Item 3
   1. Item 3a
   1. Item 3b

---
#### Images `图片`
```
格式：![Alt Text](url)
对于小白特别照顾下：  
！[图片描述](图片地址：可以是相对路径或外链地址)
例如：  
![Markdown logo](markdown.png)
![baidu logo](http://img0.bdstatic.com/static/searchresult/img/logo-2X_b99594a.png)

```
> 示例：  
![Markdown logo](markdown.png)   
![baidu logo](http://img0.bdstatic.com/static/searchresult/img/logo-2X_b99594a.png)  

----
#### Links `链接`
```
http://github.com
[GitHub](http://github.com)

链接有两种形式：
第一种就是放上直链，markdown会自动解析加上链接。
第二种 给文本加上超链接
```
> 效果如下：  

http://github.com   
[GitHub官网地址](http://github.com)

---

#### Blockquotes `引用`
用法：`>`后面 隔个空格加上文本
```
> We're living the future so
```
效果如下：  

> We're living the future so   

---
#### Inline code `内联代码`

```
用法：`代码或文本`  用两个`号包裹
I think you should use an
`<addr>` element here instead.
```
>效果如下：  

I think you should use an
`<addr>` element here instead.  

---
#### Syntax highlighting `语法高亮`  
> 常见的语言高亮支持：`js` `html` `css` `php` `python`....  

- `javascript`     
用法：在` ```js 代码块  ``` ` ，在代码块内写JS代码支持高亮效果。  

```js
function fancyAlert(arg) {
    if(arg) {
        $.facebox({div:'#foo'})
    }
}

```  
---

- `Python`  
用法和js一样 只需要把代码相应的修改成` ```py 代码块 ``` `  

```py
def foo():
    if not bar:
        return True
```  

---
- `通用代码块` - 无高亮  
写法` ``` 代码块 ``` `   

```
function People(age,sex) {
    this.age = age
    this.sex = sex
    console.log()
}
```  
---
#### Task Lists `任务列表`  
用法：`- [x]`这个是选中效果，`- [ ]`这个是没有选中。
```
- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item
```
> 效果如下：

- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported
- [x] list syntax required (any unordered or ordered list supported)
- [x] this is a complete item
- [ ] this is an incomplete item   

---
#### Tables `表格`  

```
表格头部标题一 | 表格头部标题二
------------- | -------------
内容一  | 内容二
内容三  | 内容四

```
> 效果如下    

- `三行两列`  

表格头部标题一 | 表格头部标题二
------------- | -------------
内容一  | 内容二
内容三  | 内容四  

- `四行五列`  

标题一 | 标题二 | 标题三 | 标题四 | 标题五
------ | ------ | ------ | ------ | ------
内容  | 内容  | 内容  | 内容  | 内容
内容  | 内容  | 内容  | 内容  | 内容
内容  | 内容  | 内容  | 内容  | 内容

---
#### Issue references within a repository `在存储库中发布引用`

```
#1
mojombo#1
mojombo/github-flavored-markdown#1
```
> tips： `#`号后面的数字会自动解析到你该仓库issue帖子对应的链接  

---
#### Username @mentions `@用户名`

输入`@`符号，然后输入用户名，将通知该人员来查看评论。

---
#### Strikethrough `删除线`
用法：`~~文本~~` 被双`~~`符号包裹的文本可数显删除线效果
```
Any word wrapped with two tildes (like ~~this~~) will appear crossed out.
```  
Any word wrapped with two tildes (like ~~this~~) will appear crossed out.

---
### Emoji `表情符号`
> 支持的表情符号列表 [查看表情代码](https://www.webpagefx.com/tools/emoji-cheat-sheet/)    

- 用法：使用`:`会列出建议的表情符号列表。该列表会在您键入时进行过滤，因此一旦找到了您要查找的表情符号，请按Tab或Enter键完成突出显示的结果。

@octocat :+1: This PR looks great - it's ready to merge! :shipit:

---
#### Relative links `相关链接`

您可以在渲染文件中定义相对链接和图像路径，以帮助读者导航到存储库中的其他文件。

相对链接是相对于当前文件的链接。例如，如果在存储库的根目录中有一个README文件，并且在docs / CONTRIBUTING.md中有另一个文件，则README中与CONTRIBUTING.md的相对链接可能如下所示：
```
[Contribution guidelines for this project](docs/CONTRIBUTING.md)
```
GitHub会根据您当前所在的任何分支自动转换您的相关链接或图像路径，以便链接或路径始终有效。您可以使用所有相关链接操作数，例如./和../。

对克隆存储库的用户来说，相对链接更容易。绝对链接可能无法在存储库的克隆中运行 - 我们建议使用相对链接来引用存储库中的其他文件。
> 效果如下：  

[Contribution guidelines for this project](docs/CONTRIBUTING.md)

#### 有关更多github的markdown语法请查看 [Markdown help](https://help.github.com/articles/basic-writing-and-formatting-syntax/)
