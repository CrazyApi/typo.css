# 中文网页重设与排版：TYPO.CSS
[一致化浏览器排版效果，构建最适合中文阅读的网页排版](class:tagline)

1. [关于 TYPO.CSS](#section1)
2. [排版实例](#section2)
	* [例1：论语学而篇第一](#section2-1)
	* [例2：英文排版](#section2-2)
3. [附录](#section3)
	1. [TYPO.CSS 排版偏重点](#appendix1)
	2. [开源许可](#appendix2)


## [一、关于 TYPO.CSS](id:section1)

**TYPO.CSS** 的目的是，在一致化浏览器排版效果的同时，构建最适合中文阅读的网页排版。

现状和如何去做：
排版是一个麻烦的问题，需要精心设计，而这个设计却是常被视觉设计师所忽略的。前端工程师更常看到这样的问题，但不便变更。因为在多个 OS 中的不同浏览器渲染不同，改动需要多的时间做回归测试，所以改变变得更困难。而像我们一般使用的 Yahoo、Eric Meyer 和 Alice base.css 中采用的 Reset 都没有很好地考虑中文排版。TYPO.CSS 要做的就是解决中文排版的问题。

**TYPO.CSS 测试于如下平台：**

OS/浏览器	|Firefox|Chrome|Safari|Opera|IE9|IE8|IE7|IE6
:-----------|:-----:|:----:|:----:|:---:|:-:|:-:|:-:|--:
Mac OS X	|   √   |   √  |   √  |  √  | - | - | - | -
Windows 7   |   √   |   √  |   √  |  √  | √ | √ | √ | -
Windows XP  |   √   |   √  |   √  |  √  | - | √ | √ | √
Ubuntu Linux|   √   |   √  |   -  |  √  | - | - | - | -


#### 中文排版的重点和难点

在中文排版中，HTML4 的很多标准在语义在都有照顾到。但从视觉效果上，却很难利用单独的 CSS 来实现，像[着重号](class:abbr "在文字下多加一个点")。在 HTML4 中，着重号标签（`<u>`）已经被放弃，而 HTML5 被[重新提起](http://html5doctor.com/u-element/)。TYPO.CSS 也根据实际情况提供相应的方案。我们重要要注意的两点是：

1. 语义：语义对应的用法和样式是否与中文排版一致
2. 表现：在各浏览器中的字体、大小和缩放是否如排版预期

对于这些，TYPO.CSS 排版项目的中文偏重注意点，都添加在附录中，详见：

> **附录一**：TYPO.CSS 排版偏重点

目前仍处于 alpha 开发阶段，测试平台的覆盖，特别是在[移动端](class:abbr "手机、平板电脑等移动平台")上还没有覆盖完主流平台，希望有能力的同学能加入测试行列，或者加入到 TYPO.CSS 的开发。加入方法：[参与 TYPO.CSS 开发][typo]。如有批评、建议和意见，也随时欢迎给在 Github 直接提 [issues][iss]，或给我发[邮件][mail]。

[typo]: https://github.com/sofish/typo.css
[iss]: https://github.com/sofish/typo.css/issues
[mail]: mailto:sofish@163.com

## [二、排版实例：](id:section2)

提供2个排版实例，第一个中文实例来自于来自于张燕婴的《论语》，由于古文排版涉及到的元素比较多，所以采用《论语》中《学而》的第一篇作为排版实例介绍；第2个来自到经典的 Lorem Ipsum，并加入了一些代码和列表等比较具有代表性的排版元素。

That's some text with a footnote1.[^read]

[^read]: And that's the footnote1.

### [例1：论语学而篇第一](id:section2-1)

[**作者：**[孔子](class:abbr "名丘，字仲尼")（前551年9月28日－前479年4月11日）](class:small)


#### 本篇引语

《学而》是《论语》第一篇的篇名。《论语》中各篇一般都是以第一章的前二三个字作为该篇的篇名。《学而》一篇包括16章，内容涉及诸多方面。其中重点是“吾日三省吾身”；“节用而爱人，使民以时”；“礼之用，和为贵”以及仁、孝、信等道德范畴。


#### 原文

子曰[1](#note1)：“学[2](#note2)而时习[3](#note3)之，不亦说[4](#note4)乎？有朋[5](#note5)自远方来，不亦乐[6](#note6)乎？人不知[7](#note7)，而不愠[8](#note8)，不亦君子[9](#9)乎？”

#### 注释

[1](id:note1)子：中国古代对于有地位、有学问的男子的尊称，有时也泛称男子。《论语》书中“子曰”的子，都是指孔子而言。  
[2](id:note2)学：孔子在这里所讲的“学”，主要是指学习西周的礼、乐、诗、书等传统文化典籍。  
[3](id:note3)时习：在周秦时代，“时”字用作副词，意为“在一定的时候”或者“在适当的时候”。但朱熹在《论语集注》一书中把“时”解释为“时常”。“习”，指演习礼、乐；复习诗、书。也含有温习、实习、练习的意思。  
[4](id:note4)说：音ｙｕè，同悦，愉快、高兴的意思。  
[5](id:note5)有朋：一本作“友朋”。旧注说，“同门曰朋”，即同在一位老师门下学习的叫朋，也就是志同道合的人。  
[6](id:note6)乐：与说有所区别。旧注说，悦在内心，乐则见于外。  
[7](id:note7)人不知：此句不完整，没有说出人不知道什么。缺少宾语。一般而言，知，是了解的意思。人不知，是说别人不了解自己。  
[8](id:note8)愠：音ｙùｎ，恼怒，怨恨。  
[9](id:note9)君子：《论语》书中的君子，有时指有德者，有时指有位者。此处指孔子理想中具有高尚人格的人。

其他内容在这里


#### 译文

孔子说：“学了又时常温习和练习，不是很愉快吗？有志同道合的人从远方来，不是很令人高兴的吗？人家不了解我，我也不怨恨、恼怒，不也是一个有德的君子吗？”

#### 评析

宋代著名学者[朱熹](class:u)对此章评价极高，说它是“入道之门，积德之基”。本章这三句话是人们非常熟悉的。历来的解释都是：学了以后，又时常温习和练习，不也高兴吗等等。三句话，一句一个意思，前后句子也没有什么连贯性。但也有人认为这样解释不符合原义，指出这里的“学”不是指学习，而是指学说或主张；“时”不能解为时常，而是时代或社会的意思，“习”不是温习，而是使用，引申为采用。而且，这三句话不是孤立的，而是前后相互连贯的。这三句的意思是：自己的学说，要是被社会采用了，那就太高兴了；退一步说，要是没有被社会所采用，可是很多朋友赞同我的学说，纷纷到我这里来讨论问题，我也感到快乐；再退一步说，即使社会不采用，人们也不理解我，我也不怨恨，这样做，不也就是君子吗？（见《齐鲁学刊》1986年第6期文）这种解释可以自圆其说，而且也有一定的道理，供读者在理解本章内容时参考。 此外，在对“人不知，而不愠”一句的解释中，也有人认为，“人不知”的后面没有宾语，人家不知道什么呢？当时因为孔子有说话的特定环境，他不需要说出知道什么，别人就可以理解了，却给后人留下一个谜。有人说，这一句是接上一句说的，从远方来的朋友向我求教，我告诉他，他还不懂，我却不怨恨。这样，“人不知”就是“人家不知道我所讲述的”了。这样的解释似乎有些牵强。 总之，本章提出以学习为乐事，做到人不知而不愠，反映出孔子学而不厌、诲人不倦、注重修养、严格要求自己的主张。这些思想主张在《论语》书中多处可见，有助于对第一章内容的深入了解。


### [例2：英文排版](id:section2-2)

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

> "Neque porro quisquam est qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit…"
> > "There is no one who loves pain itself, who seeks after it and wants to have it, simply because it is pain…"
>
> > "There is no one who loves pain itself, who seeks after it and wants to have it, simply because it is pain…"
> > > "There is no one who loves pain itself, who seeks after it and wants to have it, simply because it is pain…"


#### The standard Lorem Ipsum passage, used since the 1500s

"Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."


#### Section 1.10.32 of "de Finibus Bonorum et Malorum", written by Cicero in 45 BC

"Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione voluptatem sequi nesciunt. Neque porro quisquam est, qui dolorem ipsum quia dolor sit amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut labore et dolore magnam aliquam quaerat voluptatem. Ut enim ad minima veniam, quis nostrum exercitationem ullam corporis suscipit laboriosam, nisi ut aliquid ex ea commodi consequatur? Quis autem vel eum iure reprehenderit qui in ea voluptate velit esse quam nihil molestiae consequatur, vel illum qui dolorem eum fugiat quo voluptas nulla pariatur?"


#### List style in action

* If you wish to succeed, you should use persistence as your good friend, experience as your reference, prudence as your brother and hope as your sentry.
如果你希望成功，当以恒心为良友，以经验为参谋，以谨慎为兄弟，以希望为哨兵。

* Sometimes one pays most for the things one gets for nothing.
有时候一个人为不花钱得到的东西付出的代价最高。

* Only those who have the patience to do simple things perfectly ever acquire the skill to do difficult things easily.
只有有耐心圆满完成简单工作的人，才能够轻而易举的完成困难的事。

#### You may want to create a perfect `<hr />` line, despite the fact that there will never have one

---

[La Racheforcauld](class:abbr "法国作家罗切福考尔德") said: ["Few things are impossible in themselves; and it is often for want of will ,rather than of means, that man fails to succeed".](class:mark) You just need to follow the browser's behavior, and set a right `margin` to it。it will works nice as the demo you're watching now. The following code is the best way to render typo in Chinese:

```
/* 标题应该更贴紧内容，并与其他块区分，margin 值要相应做优化 */
h1,h2,h3,h4,h5,h6 {
	line-height:1;font-family:Arial,sans-serif;margin:1.4em 0 0.8em;
}
h1{font-size:1.8em;}
h2{font-size:1.6em;}
h3{font-size:1.4em;}
h4{font-size:1.2em;}
h5,h6{font-size:1em;}

/* 现代排版：保证块/段落之间的空白隔行 */
.typo p, .typo pre, .typo ul, .typo ol, .typo dl, .typo form, .typo hr{
	margin:1em 0 0.6em;
}

```

### [三、附录](id:section3)

#### [1、TYPO.CSS 排版偏重点](id:appendix1)


类型|语义|标签|注意点
:--|:--|:--|:--
基础标签|标题|h1 ～ h6|全局不强制大小，.typo 中标题与其对应的内容应紧贴，并且有相应的大小设置
|上、下标|sup/sub|保持与 MicroSoft Office Word 等程序的日常排版一致
|引用|blockquote|显示/嵌套样式
|缩写|abbr|是否都有下划线，鼠标 hover 是否为帮助手势
|分割线|hr|显示的 padding 和 margin正确
|列表|ul/ol/dl|在全局没有 list-style，在 .typo 中对齐正确
|定义列表|dl|全局 padding 和 margin为0， .typo 中对齐正确
|选项|input[type=radio[, checkbox]]|与其他 form 元素排版时是否居中
|斜体|i|只设置一种斜体，让 em 和  cite 显示为正体
|强调|em|在全局显示正体，在 .typo 中显示与 b 和 strong 的样式一致，为粗休
|加强|strong/b|显示为粗体
|标记|mark|类似荧光笔
|印刷|small|保持为正确字体的 80% 大小，颜色设置为浅灰色
|表格|table|全局不显示线条，在 table 中显示表格外框，并且表头有浅灰背景
|代码|pre/code|字体使用 courier 系字体，保持与 serif 有比较一致的显示效果
特殊符号|着重号|在文字下加点（•）|在支持 :after 和 :before 的浏览器可以做渐进增强实现
|专名号|林建锋|专名号，有下划线，使用 u 或都 .typo-u 类
|破折号|——|保持一划，而非两划
|人民币|¥|使用两平等线的符号，或者 HTML 实体符号 &yen;
|删除符|已删除（deleted）|一致化各浏览器显示，中英混排正确
加强类|专名号|.typo-u|由于 u 被 HTML4 放弃，在向后兼容上推荐使用
|着重符|.typo-em|利用 :after 和 :before 实现着重符
|首字下沉|.typo-first|特殊排版
|清除浮动|.clearfix|与一般 CSS Reset 保持一对致 API
注意点|（1）中英文混排行高/行距
|（2）上下标在 IE 中显示效果
|（3）块/段落分割空白是否符合设计原则
|（4）input 多余空间问题
|（5）默认字体色彩，目前采用 #333 在各种浏览显示比较好

##### [2、开源许可](id:appendix2)

TYPO.CSS 基于 [MIT License][mit] 开源，使用代码只需说明来源，或者引用 [license.txt][lic] 即可。

[mit]: http://zh.wikipedia.org/wiki/MIT_License
[lic]: http://typo.sofish.de/license.txt

---

**Strong**

*Emphasize*

~~Striketthought~~

`Inline Code`


 