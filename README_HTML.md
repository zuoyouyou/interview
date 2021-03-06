# HTML5
## 一 新增标签
   > 摘自[MDN](https://developer.mozilla.org/zh-CN/docs/Web/Guide/HTML/HTML5)
* 语义
> HTML5 中的区块和段落元素
> HTML5 中新的区块和段落元素一览: `<section>, <article>, <nav>, <header>, <footer>, <aside> 和 <hgroup>.`
> 使用 HTML5 的音频和视频
> `<audio>` 和 `<video>` 元素嵌入和允许操作新的多媒体内容。
* 表单的改进
> 看一下 HTML5 中对 web 表单的改进：强制校验API，一些新的属性，一些新的`<input`> 元素type 属性值 ，新的 `<output>` 元素。
* 新的语义元素
> 除了节段，媒体和表单元素之外，还有众多的新元素，例如 `<mark>， <figure>， <figcaption>， <data>， <time>， <output>， <progress>`， 或者 `<meter>`和`<main>`，这增加了有效的 HTML5 元素的数量。
* <iframe> 的改进
> 使用 sandbox， seamless， 和 srcdoc 属性，作者们现在可以精确控制 `<iframe>` 元素的安全级别以及期望的渲染。
### 在不支持HTML5的浏览器器中使用HTML5
  * way1: 
   
      ```
      section, article, aside, footer, header, nav, hgroup {
        display:block;
      }
      ```
  * way2(ie8及以下不支持改变不支持的元素的样式):
      
      ```
         <!--[if lt IE 9]>
           <script>
             document.createElement("header" );
             document.createElement("footer" );
             document.createElement("section"); 
             document.createElement("aside"  );
             document.createElement("nav"    );
             document.createElement("article"); 
             document.createElement("hgroup" ); 
             document.createElement("time"   );
           </script>
           <noscript>
              <strong>Warning !</strong>
              Because your browser does not support HTML5, some elements are simulated using JScript.
              Unfortunately your browser has disabled scripting. Please enable it in order to display this page.
           </noscript>
         <![endif]-->
      ```
## 二 杂项
* Doctype作用? 严格模式？混杂模式？
   
   ```
   <!DOCTYPE>声明在HTML最前面，告知浏览器的解析器，用什么文档类型规范来解析这个文档。
   严格模式的排版和JS运作模式是以该浏览器支持的最高标准运行。
   在混杂模式中，页面以宽松的向后兼容的方式显示。模拟老式浏览器的行为以防止站点无法工作。
   ```
   ***
* 块级元素？内联元素？空元素？
  * 块级元素
  `div ul ol li dl dt dd h1 h2 h3 h4 p `
  * 内联元素
  `a b span img input select strong`
  * 空元素(即没有内容的HTML元素)
  `<img> <link> <meta> <br> <hr>`
     
