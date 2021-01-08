# 欢迎使用 MPEditor Markdown 编辑器

**MPEditor**是专注于微信公众号的编辑阅读器，利用 MPEditor 可以使用 **Markdown** 语法编写微信公众号文章，编辑完后可以复制到公众号发布平台直接发布，真正的实现即看即所得：

-   更加贴合微信 UI 标准
-   支持实时预览
-   支持同步滚动
-   支持语法高亮
-   支持 emoji 表情

> MPEditor 解决了微信公众号编辑中遇见的一些编辑问题，增加了「工（ma）程（nong）师（men）」经常遇见的代码高亮、emoji 问题。希望你会喜欢这种极（zhuang）客（bi）的体验

==[header-box] 使用方法

在左侧Markdown编辑器中编写Markdown格式的内容，编辑完成后点击右上角`√`，复制内容到微信编辑器粘贴即可。

## 本编辑器支持快捷键

-   `⌘+S` or `Ctrl+S`：保存编写的内容

==[header-box]  什么是 Markdown

Markdown 是一种方便记忆、书写的纯文本标记语言，用户可以使用这些标记符号以最小的输入代价生成极富表现力的文档：譬如您正在阅读的这份文档。它使用简单的符号标记不同的标题，分割不同的段落，**粗体** 、 _斜体_ 、~~delete~~ 某些文字。["info" MPEditor] 使用了 `showdown` 语法（一种 markdown 的扩展语法）

==[header-box]  语法


## 标题二

### 标题三

#### 标题四

##### 标题五，不常用

###### 标题六，不常用

## 1. 基本列表样式

-   偶是个无序列表
    -   我是个二级无序列表
-   真巧啊我也是个无序列表

1. 我是个有序列表啊
2. 嗯，me too~
3. markdown so easy! 妈妈再也不用担心我的**学习**了

!> 由于微信原因，最多支持到二级列表。
## 2. 高亮一段代码
使用了微信原生语法高亮。
```js
// 新语法检测
import $ from 'jQuery';
$(document).on('click', () => {
    let that = this;
    console.log(that);
});

var aceEditor = new ace.editor('#id');

$(function () {
    $('div').html('I am a div.');
});
```

上面是 `JavaScript`，下面是 `php`：

```php
echo 'hello,world'
```

## 3. 链接和图片

-   MPEditor：https://github.com/ksky521/mpeditor
-   demo: [点击查看 demo](https://github.com/ksky521/mpeditor/blob/master/static/demo.md)

下面是个「三水清」的微信公众号二维码，欢迎扫描关注：
![关注三水清](https://wx3.sinaimg.cn/orj360/796f423bly1gfzytdw3qhj20by0byq3p.jpg)

换个小点的头像
![关注三水清](https://wx3.sinaimg.cn/orj360/796f423bly1gfzytdw3qhj20by0byq3p.jpg =120x120)

## 4. 支持 emoji！

-   Unicode 支持：😈 💗 😄 🐂 👍
-   github 版本支持： :cn: :red_car: :muscle: :smile: :sunglasses:

## 5. 绘制表格

下面是个普通的表格
| 公众号 | id | 备注 |
|:-----|-----|:------:|
| 三水清 | sanshuiqing123 | 作者很帅 |
| 博客 | http://js8.in | 程序媛鼓励师 |

支持另外一种语法：
公众号 | id/网址 | 备注
------------ | ---------- | ------
三水清 | sanshuiqing123 | 作者很帅
博客 | http://js8.in | 程序媛鼓励师

## 6. 扩展`inline`语法样式

此部分写法，会被转换为`span`包裹的文字，然后加上对应的样式属性

### 颜色扩展

-   ["green" 内置绿色 green/success]
-   ["danger" 内置红色 danger/red]
-   ["blue" 蓝色 info/blue]
-   ["warning" 黄色 warning/yellow]
-   ["#ccc" 自定义颜色值#ccc] + ["#337ab7" 自定义颜色值#337ab7]

### 字号扩展

-   ["12px" 自定义字号 12px]
-   ["120%" 自定义字号 120%]
-   ["2em" 自定义字号 2em]

### 任意自定义样式组合

-   ["padding-left:20px;color: red;" 自定义 css 样式]

## 7. 引用

> MPEditor 解决了微信公众号编辑中遇见的一些编辑问题，增加了「工（ma）程（nong）师（men）」经常遇见的代码高亮、emoji 问题。希望你会喜欢这种极（zhuang）客（bi）的体验

下面是个特殊的引用，背景是红色

!> MPEditor 解决了微信公众号编辑中遇见的一些编辑问题，增加了「工（ma）程（nong）师（men）」经常遇见的代码高亮、emoji 问题。希望你会喜欢这种极（zhuang）客（bi）的体验

### 3.6 引用

引用的格式是在符号 `>` 后面书写文字，文字的内容可以包含标题、链接、图片、粗体和斜体等。

一级引用如下：

> ### 一级引用示例
> 
> 读一本好书，就是在和高尚的人谈话。 **——歌德**
> 
> [Markdown Nice最全功能介绍](https://mp.weixin.qq.com/s/lM808MxUu6tp8zU8SBu3sg)
> 
> ![这里写图片描述](https://files.mdnice.com/pic/cd3ca20c-896f-4cfc-9bdd-c4c58e69ba26.jpg)

当使用多个 `>` 符号时，就会变成多级引用

二级引用如下：

>> ### 二级引用示例
>>
>> 读一本好书，就是在和高尚的人谈话。 **——歌德**
>>
>> [Markdown Nice最全功能介绍](https://mp.weixin.qq.com/s/lM808MxUu6tp8zU8SBu3sg)
>> 
>> ![这里写图片描述](https://files.mdnice.com/pic/cd3ca20c-896f-4cfc-9bdd-c4c58e69ba26.jpg)

三级引用如下：

>>> ### 三级引用示例
>>>
>>> 读一本好书，就是在和高尚的人谈话。 **——歌德**
>>>
>>> [Markdown Nice最全功能介绍](https://mp.weixin.qq.com/s/lM808MxUu6tp8zU8SBu3sg)
>>> 
>>> ![这里写图片描述](https://files.mdnice.com/pic/cd3ca20c-896f-4cfc-9bdd-c4c58e69ba26.jpg)

## 8. 分割线

--分割线--

==密封线==

## 9. 内置样式

?> 下面是一些特殊样式，你可能用得到

1. 盒子标题
===[header-box] 盒子标题

2. 数字标题
===[header-num] 01. 这是标题

3. 主副标题文字
===[header-num] 副标题. 这里是主标题

4. 底部扫码盒子

===[qrcode-box]



再一次感谢您花费时间阅读这份欢迎稿！

--EOF--

~~~font-size: 12px;

作者[@三水清](http://weibo.com/sanshuiqing)
2020 年 06 月 21 日

[center]下面是个「三水清」的微信公众号二维码，欢迎扫描关注：
![关注三水清](https://wx3.sinaimg.cn/orj360/796f423bly1gfzytdw3qhj20by0byq3p.jpg)[/center]

~~~

~~~display: flex;justify-content:center;align-items:center;
![关注三水清](https://wx3.sinaimg.cn/orj360/796f423bly1gfzytdw3qhj20by0byq3p.jpg  =120x120)

![关注三水清](https://wx3.sinaimg.cn/orj360/796f423bly1gfzytdw3qhj20by0byq3p.jpg =120x120)
~~~
