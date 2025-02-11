---
title: html-interview
topic: 
type: D
tags:
  - CSS
category: 
Datereviewed: 
reviewed: 
difficulty: 
status: 
comment: 
draft: true
DateStarted: 2024-04-25
DateModified: 2024-04-25
---
### DOCTYPE 有什么作用？

DOCTYPE 是一种指示浏览器以何种 HTML 或 XHTML 规范来解析文档的声明。它能够告知浏览器网页文档使用的标记语言的类型以及版本，从而确保浏览器能够正确地展示网页内容。DOCTYPE 声明通常位于 HTML 文档的开头，是 HTML 文档的必须部分。

### img 标签的 title 和 alt 属性有什么区别

`alt`属性用于为图像提供替代文本，即使图像无法加载，也可以描述图像内容，提高网页的可访问性和可用性。`title`属性则提供有关图像的额外信息，可以通过鼠标悬停或使用辅助技术来查看。它通常用于提供更多的上下文或补充描述，但并不是必需的。

### 简述一下 src 与 href 的区别

在 HTML 中，`src` 属性是用来指定外部资源的 URL，如图像、脚本或嵌入式对象的位置。例如，`<img>` 标签中的 `src` 属性指定图像的 URL。

而 `href` 属性则用来指定超文本链接的目标资源的位置，如超链接或 `link` 标记中的外部样式表。例如，`<a>` 标签中的 `href` 属性指定了链接目标的 URL。

### iframe 有哪些优缺点？

`iframe`（内联框架）是一种 HTML 元素，它允许在当前文档中嵌入另一个独立的 HTML 文档。`iframe` 有一些优点和缺点：

优点：

1. **内容隔离**：`iframe` 可以将不同来源的内容隔离开来，使得它们在不同的上下文中运行。这有助于保护当前文档免受潜在的安全风险，并确保不同来源的内容不会互相干扰。
2. **异步加载**：`iframe` 中的内容可以异步加载，这意味着页面主体内容可以在 `iframe` 加载完成之前呈现。这有助于提高页面加载速度。
3. **独立滚动**：`iframe` 内的内容可以独立滚动，而不会影响主页面的滚动。这有助于在需要展示大量内容的情况下，提高用户体验。
4. **跨域资源访问**：在一定程度上，`iframe` 可以用于访问跨域资源，例如嵌入来自其他域的网页或应用。

缺点：

1. **性能影响**：`iframe` 的使用可能会导致性能下降，因为它需要浏览器加载额外的文档资源。每个嵌入的 `iframe` 都需要额外的 HTTP 请求，这可能会延长页面加载时间。
2. **复杂性增加**：`iframe` 的使用可能会使页面结构更加复杂，导致维护困难。而且，在 `iframe` 和主页面之间进行通信可能会涉及到跨域问题，这会增加开发难度。
3. **SEO 不友好**：搜索引擎可能无法完全索引 `iframe` 中的内容，这会影响到网页的搜索引擎优化（SEO）。
4. **可访问性问题**：`iframe` 在某些情况下可能导致可访问性问题。例如，屏幕阅读器可能无法正确解析 `iframe` 中的内容，导致部分用户无法访问这些内容。

综上所述，`iframe` 有一些优点，如内容隔离、异步加载和独立滚动等。然而，它也有一些缺点，如性能影响、复杂性增加、SEO 不友好和可访问性问题等。在使用 `iframe` 时，需要权衡这些优缺点，确保它适用于你的需求。

### 常用的 meta 标签有哪些？

`meta` 标签提供了有关 HTML 文档的元数据，如描述、关键词、作者等。以下是一些常用的 `meta` 标签：

1. **字符集声明**：声明文档使用的字符编码，通常为 UTF-8。

   ```html
   <meta charset="UTF-8" />
   ```

2. **视口设置**：控制页面在移动设备上的显示方式，如缩放级别和页面宽度。

   ```html
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   ```

3. **页面描述**：提供页面的简短描述，有助于搜索引擎了解页面内容。

   ```html
   <meta name="description" content="A brief description of the page." />
   ```

4. **关键词**：设置页面关键词，有助于搜索引擎优化（SEO）。但请注意，大多数现代搜索引擎不再使用此标签。

   ```html
   <meta name="keywords" content="keyword1, keyword2, keyword3" />
   ```

5. **作者**：指定页面作者。

   ```html
   <meta name="author" content="Author Name" />
   ```

6. **禁止缓存**：告诉浏览器不要缓存页面。

   ```html
   <meta
   	http-equiv="Cache-Control"
   	content="no-cache, no-store, must-revalidate"
   />
   <meta http-equiv="Pragma" content="no-cache" />
   <meta http-equiv="Expires" content="0" />
   ```

7. **自动刷新**：设置页面在特定时间间隔后自动刷新。

   ```html
   <meta http-equiv="refresh" content="30" />
   ```

8. **跳转到其他页面**：在指定的时间间隔后，自动将用户重定向到其他页面。

   ```html
   <meta
   	http-equiv="refresh"
   	content="5; URL=https://example.com/new-page.html"
   />
   ```

9. **兼容模式**：指定浏览器（如 Internet Explorer）使用特定的渲染模式。

   ```html
   <meta http-equiv="X-UA-Compatible" content="IE=edge" />
   ```

10. **搜索引擎索引控制**：指示搜索引擎是否应索引页面和跟踪链接。

    ```html
    <meta name="robots" content="index, follow" />
    ```

这些常用的 `meta` 标签可以帮助你控制页面的显示、搜索引擎优化和其他功能。根据页面需求，可以根据需要添加更多的 `meta` 标签。

### H5 和 H4 有什么不同？

- 语义化标签: `header`、`footer`、`nav`、`section`、`article`、`aside` 等
- 增强型表单：`date`(从一个日期选择器选择一个日期) 、`email`(包含 e-mail 地址的输入域) 、`number`(数值的输入域) 、`range`(一定范围内数字值的输入域) 、`search`(用于搜索域) 、`tel`(定义输入电话号码字段) 等
- 视频和音频：`audio`、`video`
- `Canvas`绘图、 `SVG`绘图
- 地理定位：`Geolocation`
- 拖放 API：`drag`
- `web worker`：是运行在后台的 `JavaScript`，独立于其他脚本，不会影响页面的性能
- `web storage`: `localStorage`、`sessionStorage`
- `WebSocket`: `HTML5` 开始提供的一种在单个 `TCP` 连接上进行全双工通讯的协议

### SVG 和 CANVAS 的区别？

SVG 和 Canvas 都是用于在 web 上绘制图形的技术，但它们有几个主要区别:

1. SVG 是基于矢量图的，而 Canvas 是基于像素图的。
2. 在 SVG 中，每个绘制的元素都是一个独立的 DOM 对象，并且可以轻松地与 JavaScript 交互。 在 Canvas 中，所有绘制都被放置在一个画布中，并且只能与像素级别进行交互。
3. SVG 通常适用于静态图形，而 Canvas 适用于动态图形，例如游戏和数据可视化。

简而言之，SVG 适用于需要与 DOM 交互并具有复杂动画和交互的情况，而 Canvas 则适用于创建大量图形对象和复杂动画。

### defer 和 async 的区别 ?

defer 和 async 都是用于脚本加载和执行的关键字，两者的主要区别如下：

1. defer 脚本会在 HTML 文档解析完成后执行，而 async 脚本会在下载完毕后立即执行。
2. defer 脚本会按照它们在文档中的顺序执行，而 async 脚本是在下载完成后尽快执行，可能会打乱它们在文档中的顺序。
3. defer 脚本会在 DOMContentLoaded 事件之后运行，而 async 脚本则不一定。

因此，如果需要按顺序执行脚本并且不想阻塞 DOM 的解析，可以使用 defer。如果脚本的执行不依赖于其他脚本或 DOM，可以使用 async 加快加载速度。

### style 标签 prefetch 和 preload 区别？

`<style>`标签的`prefetch`和`preload`属性都用于优化 CSS 资源的加载，但它们有不同的行为和目的：

- `prefetch`属性告诉浏览器这个 CSS 资源可能在未来的某个时刻需要被加载，但并不需要立即加载。浏览器会在空闲时间异步加载这个资源，以便在需要时能够立即使用。`prefetch`适用于那些当前不需要但是可能在未来会需要使用的资源。
- `preload`属性则告诉浏览器这个 CSS 资源在当前页面中必须被使用，因此应该立即加载和执行。浏览器会在主 HTML 文档下载和解析完成之前加载这个资源。`preload`适用于那些当前需要使用的资源。
### 3.XHTML和HTML有什么区别？

一、其基础语言不同

1、XhtmL是基于可扩展标记语言（XmL）。

2、htmL是基于标准通用标记语言（sgmL）。

二、语法严格程度不同

1、XhtmL语法比较严格，存在dtd定义规则。

2、htmL语法要求比较松散，这样对网页编写者来说，比较方便。

三、可混合应用不同

1、XhtmL可以混合各种XmL应用，比如mathmL、sVg。

2、htmL不能混合其它XmL应用。

四、大小写敏感度不同

1、XhtmL对大小写敏感，标准的XhtmL标签应该使用小写。

2、htmL对大小写不敏感。

五、公布时间不同

1、XhtmL是2000年w3c公布发行的。

2、htmL4.01是1999年w3c推荐标准。

### 4.Doctype? 严格模式与混杂模式-如何触发这两种模式？

严格模式与混杂模式——如何触发这两种模式，区分它们有何意义。

在标准模式中，浏览器根据规范呈现页面；

在混杂模式中，页面以一种比较宽松的向后兼容的方式显示。

浏览器根据DOCTYPE是否存在以及使用的哪种DTD来选择要使用的呈现方法。如果XHTML文档包含形式完整的DOCTYPE，那么它一般以标准模式呈现。对于HTML 4.01文档，包含严格DTD的DOCTYPE常常导致页面以标准模式呈现。包含过渡DTD和URI的DOCTYPE也导致页面以标准模式呈现，但是有过渡DTD而没有URI会导致页面以混杂模式呈现。DOCTYPE不存在或形式不正确会导致HTML和XHTML文档以混杂模式呈现。

声明位于文档中的最前面的位置，处于 标签之前。此标签可告知浏览器文档使用哪种 HTML 或 XHTML 规范。

该标签可声明三种 DTD 类型，分别表示严格版本、过渡版本以及基于框架的 HTML 文档

1. 浏览器模式

当浏览器厂商开始创建与标准兼容的浏览器时，他们希望确保向后兼容性。为了实现这一点，他们创建了两种呈现模式：标准模式和混杂模式（quirks mode）。在标准模式中，浏览器根据规范呈现页面；在混杂模式中，页面以一种比较宽松的向后兼容的方式显示。混杂模式通常模拟老式浏览器（比如Microsoft IE 4和Netscape Navigator 4）的行为以防止老站点无法工作。

Mozilla和Safari还有第三种模式，称为”几乎标准的模式（almost standards mode）”，除了在处理表格的方式上有一些细微的差异之外，这种模式与标准模式相同。

在Firefox中，可以使用Web Developer Extension查看页面的呈现模式。如果网站以标准模式呈现，工具栏上会显示一个绿色的钩；若以混杂模式呈现，则显于红色的叉。IE 8中的开发工具也显示浏览器使用的模式。

差异：

对于这两种模式之间的差异，最显著的一个例子与Windows上IE专有的盒模型有关。在IE 6出现时，在标准模式中使用的是正确的盒模型，在混杂模式中使用的则是老式的专有盒模型。为了维持对IE 5和更低版本的向后兼容性，Opera 7和更高版本也在混杂模式中使用有缺点的IE盒模型。

呈现方面的其他差异比较小，而且是与特定浏览器相关的，包括对于十六进制颜色值不需要#号、假设CSS中没有指定单位的长度的单位是像素，以及在使用关键字时将字号增加一级。

2：如何触发这两种模式:

浏览器根据DOCTYPE是否存在以及使用的哪种DTD来选择要使用的呈现方法。如果XHTML文档包含形式完整的DOCTYPE，那么它一般以标准模式呈现。对于HTML 4.01文档，包含严格DTD的DOCTYPE常常导致页面以标准模式呈现。包含过渡DTD和URI的DOCTYPE也导致页面以标准模式呈现，但是有过渡DTD而没有URI会导致页面以混杂模式呈现。DOCTYPE不存在或形式不正确会导致HTML和XHTML文档以混杂模式呈现。

根据DOCTYPE是否存在选择呈现模式，被称为DOCTYPE切换或DOCTYPE侦测。并非所有浏览器都采用这些规则，但是这些规则很好地说明了DOCTYPE切换的工作方式。要了解更全面的内容，可查阅网站http://hsivonen.iki.fi/doctype/，这里的图表说明了不同浏览器如何根据DOCTYPE声明来选择呈现方法。

DOCTYPE切换是浏览器用来区分遗留文档和符合标准的文档的手段。无论是否编写了有效的CSS，如果选择了错误的DOCTYPE，那么页面就将以混杂模式呈现，其行为就可能会有错误或不可预测。因此，一定要在站点的每个页面上包含形式完整的DOCTYPE声明，并且在使用HTML时选择严格的DTD。
### 1、什么是HTML语义化？
基本上都是围绕着几个主要的标签，像标题（H1~H6）、列表（li）、强调（strong em）等等  
　　根据内容的结构化（内容语义化），选择合适的标签（代码语义化）便于开发者阅读和写出更优雅的代码的同时让浏览器的爬虫和机器很好地解析。  
2、为什么要语义化？  
为了在没有CSS的情况下，页面也能呈现出很好地内容结构、代码结构:为了裸奔时好看；  
用户体验：例如title、alt用于解释名词或解释图片信息、label标签的活用；  
有利于SEO：和搜索引擎建立良好沟通，有助于爬虫抓取更多的有效信息：爬虫依赖于标签来确定上下文和各个关键字的权重；  
方便其他设备解析（如屏幕阅读器、盲人阅读器、移动设备）以意义的方式来渲染网页；  
便于团队开发和维护，语义化更具可读性，是下一步吧网页的重要动向，遵循W3C标准的团队都遵循这个标准，可以减少差异化。  
1，去掉或者丢失样式的时候能够让页面呈现出清晰的结构  
2，有利于SEO：和搜索引擎建立良好沟通，有助于爬虫抓取更多的有效信息：爬虫依赖于标签来确定上下文和各个关键字的权重；  
3，方便其他设备解析（如屏幕阅读器、盲人阅读器、移动设备）以意义的方式来渲染网页；  
4，便于团队开发和维护，语义化更具可读性，是下一步吧网页的重要动向，遵循W3C标准的团队都遵循这个标准，可以减少差异化。
### 3、写HTML代码时应注意什么？
尽可能少的使用无语义的标签p和span；  
在语义不明显时，既可以使用p或者p时，尽量用p, 因为p在默认情况下有上下间距，对兼容特殊终端有利；  
不要使用纯样式标签，如：b、font、u等，改用css设置。  
需要强调的文本，可以包含在strong或者em标签中（浏览器预设样式，能用CSS指定就不用他们），strong默认样式是加粗（不要用b），em是斜体（不用i）；  
使用表格时，标题要用caption，表头用thead，主体部分用tbody包围，尾部用tfoot包围。表头和一般单元格要区分开，表头用th，单元格用td；  
表单域要用fieldset标签包起来，并用legend标签说明表单的用途；  
每个input标签对应的说明文本都需要使用label标签，并且通过为input设置id属性，在lable标签中设置for=someld来让说明文本和相对应的input关联起来。

### 9.Doctype作用？标准模式与兼容模式各有什么区别?

!DOCTYPE声明位于位于HTML文档中的第一行，处于html 标签之前。告知浏览器的解析器用什么文档标准解析这个文档。DOCTYPE不存在或格式不正确会导致文档以兼容模式呈现。  
标准模式的排版 和JS运作模式都是以该浏览器支持的最高标准运行。在兼容模式中，页面以宽松的向后兼容的方式显示,模拟老式浏览器的行为以防止站点无法工作。

### 16. XML和JSON的区别？

(1).数据体积方面。  
JSON相对于XML来讲，数据的体积小，传递的速度更快些。  
(2).数据交互方面。  
JSON与JavaScript的交互更加方便，更容易解析处理，更好的数据交互。  
(3).数据描述方面。JSON对数据的描述性比XML较差。  
(4).传输速度方面。JSON的速度要远远快于XML。

### 32.关于Web端iframe有那些优缺点？

1、缺点：  
在网页中使用框架结构最大的弊病是搜索引擎的"蜘蛛"程序无法解读这种页面。当"蜘蛛"程序遇到由数个框架组成的网页时，它们只看到框架而无法找到链 接，因此它们会以为该网站是个死站点，并且很快转身离去。对一个网站来说这无异于一场灾难。如果你想销售产品，你需要客户;如想得到客户，你首先要让人们 访问你的网站，而要做到这一点，你就非求助于搜索引擎不可。你花费了大量的时间、精力和金钱开设了一家网上商店，却又故意不让搜索引擎检索你，这就好象开 家零售商店，却将窗户全部漆成黑色，而且还不挂任何招牌一样。

2、优点：  
从上文中我们可以发现，使用ifame框架的弊端是无法被搜索引擎所爬行抓取。但凡事总是具有两面性。它的这个缺点也可能是他的优点。利用这一点那我 们就可以把我们站点上一些需要给我们的用户查看，但是不需要搜索引擎爬行的内容用ifame框架进行显示，这样就可以让ifram发挥真正的效果了，而且 有我们站点中的代码也可以得到很大的精简，举一个例子，就如笔者上文提到的添加微博直播信息，这些微博信息我们并不需要提供给搜索引擎，而我们需要提供的 是与访客的一个互动的体验，如下图所示，而如果我们使用ifame框架嵌入微博的信息，不仅可以简便的添加站点的微博直播平台，同时我们看到代码也十分的 精简。

iframe好在能够把原先的网页全部原封不动显示下来,但是如果用在首页,是搜索引擎最套讨厌的.那么你的网站即使做的在好,也排不到好的名次!如 果是动态网页，用include还好点！但是必须要去除他的


