# Markdown教程
这是Markdown文档编写教程。

创建于2025年11月8日

## 1.Markdown 标题语法

要创建标题，请在单词或短语前面添加井号 (#) 。 “#” 的数量代表了标题的级别。 例如，添加三个 # 表示创建一个三级标题 。

	
# Heading level 1
## Heading level 2
### Heading level 3
#### Heading level 4
##### Heading level 5
###### Heading level 6		

还可以在文本下方添加任意数量的 == 号来标识一级标题，或者 -- 号来标识二级标题。


## 2.Markdown 段落语法

要创建段落，请使用空白行将一行或多行文本进行分隔。  
I really like using Markdown.  
I think I'll use it to 
format all of my documents from now on.

**不要用空格（spaces）或制表符（ tabs）缩进段落。**

## 3.Markdown 换行语法
在一行的末尾添加两个或多个空格，然后按回车键,即可创建一个换行。   
This is the first line.  
And this is the second line.  

为了兼容性，请在行尾添加“结尾空格”或 HTML 的 <br> 标签来实现换行。   
This is the first line.<br>
And this is the second line.  

## 4.Markdown强调语法
### 4.1粗体
通过将文本设置为粗体或斜体来强调其重要性。  

要加粗文本，请在单词或短语的前后各添加两个星号（**）或下划线（__）。  

如需加粗一个单词或短语的中间部分用以表示强调的话，请在要加粗部分的两侧各添加两个星号。  

I just love **bold text**.  
I just love __bold text__.

### 4.2斜体
要用斜体显示文本，请在单词或短语前后添加一个星号（*）或下划线（_）。  
要斜体突出单词的中间部分，请在字母前后各添加一个星号，中间不要带空格。  

I just love *bold text*.   
I just love _bold text_.

### 4.3粗体和斜体
要同时用粗体和斜体突出显示文本，请在单词或短语的前后各添加三个星号或下划线。  
要加粗并用斜体显示单词或短语的中间部分，请在要突出显示的部分前后各添加三个星号，中间不要带空格。  
This text is ***really important***.  
This text is ___really important___.  
This text is __*really important*__.  
This text is **_really important_**.  
This is really ***very*** important text.

## 5.Markdown引用语法
要创建块引用，请在段落前添加一个 > 符号。  
> Dorothy followed her through many of the beautiful rooms in her castle.  

块引用可以包含多个段落。为段落之间的空白行添加一个 > 符号。

> Dorothy followed her through many of the beautiful rooms in her castle.
>
> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

块引用可以嵌套。在要嵌套的段落前添加一个 >> 符号。

> Dorothy followed her through many of the beautiful rooms in her castle.
>
>> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.

块引用可以包含其他 Markdown 格式的元素。但是不是所有元素都可以使用。
> #### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
>  *Everything* is going according to **plan**.

## 6.Markdown列表语法
### 6.1有序列表
要创建有序列表，请在每个列表项前添加数字并紧跟一个英文句点。数字不必按数学顺序排列，但是列表应当以数字 1 起始。
1. First item
2. Second item
3. Third item
4. Fourth item

需要注意列表的数字是顺序，无论是否顺序标注。
1. First item
1. Second item
1. Third item
1. Fourth item


1. First item
8. Second item
3. Third item
5. Fourth item

嵌套列表，使用tab进行缩进后再进行。
1. First item
2. Second item
    1. haha
3. Third item
    1. Indented item
        1. heihei
    2. Indented item
4. Fourth item

### 6.2无序列表
要创建无序列表，请在每个列表项前面添加破折号 (-)、星号 (*) 或加号 (+) 。缩进一个或多个列表项可创建嵌套列表。  
- First item
- Second item
- Third item
- Fourth item

* First item
* Second item
* Third item
* Fourth item

+ First item
+ Second item
+ Third item
+ Fourth item

- First item
- Second item
- Third item
    - Indented item
        * haha
    - Indented item
- Fourth item

### 6.3在列表中嵌套其他元素
要在保留列表连续性的同时在列表中添加另一种元素，请将该元素缩进四个空格或一个制表符，如下例所示：  
嵌套段落：
*   This is the first list item.
*   Here's the second list item.

    I need to add another paragraph below the second list item.

*   And here's the third list item.

嵌套引用快：
*   This is the first list item.
*   Here's the second list item.

    > A blockquote would look great below the second list item.

*   And here's the third list item.

嵌套代码块：  
代码块通常采用四个空格或一个制表符缩进。当它们被放在列表中时，请将它们缩进八个空格或两个制表符。
1.  Open the file.
2.  Find the following code block on line 21:

        &lt;html>
          &lt;head>
            &lt;title>Test&lt;/title>
          &lt;/head>

3.  Update the title to match the name of your website.


嵌套列表：
1. First item
2. Second item
3. Third item
    - Indented item
    - Indented item
4. Fourth item


## 7.Markdown代码语法
要将单词或短语表示为代码，请将其包裹在反引号中。  
At the command prompt, type `nano`.

如果你要表示为代码的单词或短语中包含一个或多个反引号，则可以通过将单词或短语包裹在双反引号中。  
``Use `code` in your Markdown file.``

要创建代码块，请将代码块的每一行缩进至少四个空格或一个制表符。  

    &lt;html>
      &lt;head>
      &lt;/head>
    &lt;/html>

要创建不用缩进的代码块，可以使用***围栏式代码块（fenced code blocks）***.  
在代码块之前和之后的行上使用三个反引号（(```）或三个波浪号（~~~）。  
```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```
~~~
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
~~~
为编写代码的任何语言添加颜色突出显示。要添加语法突出显示，请在受防护的代码块之前的反引号旁边指定一种语言。

```json
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

```python
print("hello world!")
```

## 8.Markdown分割线语法

要创建分隔线，请在单独一行上使用三个或多个星号 (***)、破折号 (---) 或下划线 (___) ，并且不能包含其他内容。  

*****

-----
________________


## 9.Markdown链接语法
链接文本放在中括号内，链接地址放在后面的括号中，链接title可选。

超链接Markdown语法代码：[超链接显示名](超链接地址 "超链接title")

这是一个链接 [Markdown语法](https://markdown.com.cn)。

链接title是当鼠标悬停在链接上时会出现的文字，这个title是可选的，它放在圆括号中链接地址后面，跟链接地址之间以空格分隔。

这是一个链接 [Markdown语法](https://markdown.com.cn "最好的markdown教程")。

使用尖括号可以很方便地把URL或者email地址变成可点击的链接。

<https://markdown.com.cn> 

<25126576@bjtu.edu.cn>

强调 链接, 在链接语法前后增加星号。 要将链接表示为代码，请在方括号中添加反引号。

I love supporting the **[EFF](https://eff.org)**.  
This is the *[Markdown Guide](https://www.markdownguide.org)*.  
See the section on [`code`](#code).

## 10.Markdown图片语法
要添加图像，请使用感叹号 (!), 然后在方括号增加替代文本，图片链接放在圆括号里，括号里的链接后可以增加一个可选的图片标题文本。

插入图片Markdown语法代码：![图片alt](README/Markdown_images/屏保1.jpg "图片title")

给图片增加链接，请将图像的Markdown 括在方括号中，然后将链接添加在圆括号中。

[![沙漠中的岩石图片](/assets/img/shiprock.jpg "Shiprock")](https://markdown.com.cn)

## 11.Markdown 表格语法
要添加表，请使用三个或多个连字符（---）创建每列的标题，并使用管道（|）分隔每列。您可以选择在表的任一端添加管道。

| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |

单元格宽度可以变化。

您可以通过在标题行中的连字符的左侧，右侧或两侧添加冒号（:），将列中的文本对齐到左侧，右侧或中心。

| Syntax      | Description | Test Text     |
| :---        |    :----:   |          ---: |
| Header      | Title       | Here's this   |
| Paragraph   | Text        | And more      |

请尝试使用 [Markdown Tables Generator](https://www.tablesgenerator.com/markdown_tables)。使用图形界面构建表，然后将生成的Markdown格式的文本复制到文件中。


## 12.Markdown删除线
您可以通过在单词中心放置一条水平线来删除单词。结果看起来像这样。此功能使您可以指示某些单词是一个错误，要从文档中删除。若要删除单词，请在单词前后使用两个波浪号~~。

~~世界是平坦的。~~ 我们现在知道世界是圆的。

## 13.Markdown 任务列表语法
任务列表使您可以创建带有复选框的项目列表。在支持任务列表的Markdown应用程序中，复选框将显示在内容旁边。要创建任务列表，请在任务列表项之前添加破折号-和方括号[ ]，并在[ ]前面加上空格。要选择一个复选框，请在方括号[x]之间添加 x 。

- [x] Write the press release
- [x] Update the website
- [ ] Contact the media
