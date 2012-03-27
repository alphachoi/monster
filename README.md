# Monster
Monster是Alipay UED推出的网站代码分析、质量检测及评分的浏览器扩展，它能智能分析CSS、JS、HTML内容并生动形象展示网页得分情况(类似YSlow)。
它是一个开源项目，您可以在GoogleCode中心检出MonsterForChrome项目源代码。不久会推出Firefox版扩展。

##### 下载及演示
* [下载Monster](https://chrome.google.com/extensions/detail/dcnccmmdjdapgpnjhdakbjdncokmgonf)
* [视频演示(低质量)](http://v.youku.com/v_show/id_XMTcwNDg2Mjgw.html)

### Monster主要检测规则：
* 检测是否有重复ID的标签；
* 检测是否使用内联标签嵌套块级标签，如a嵌套div；
* 检测https协议页面，是否使用了http协议的图片、JS、CSS等；
* 检测compatMode、doctype是否出错；
* 检测是否使用了HTML5不再支持的标记，如font,s,u等；
* 检测标签是否正确关闭；
* 检测CSS、JS、background-image文件是否为404；
* 检测CSS、JS文件是否重复调用；
* 检测是否引用过多外部JS、CSS文件；
* 检测CSS、JS、HTML是否压缩；
* 检测CSS样式表是否使用了CSS expression；
* 检测Cookie是否超过30KB；
* 检测是否有form标签嵌套form标签；
* 检测是否直接在标签里定义JS事件，如 &lt;a href=”#” onclick=”…”&gt;link&lt;/a&gt;；
* 检测 &lt;meta charset=”utf-8″ /&gt; 是否为&lt;head&gt;第一个子标签；
* 检测一个 &lt;form&gt; 标签内部是否出现二个 input[type=submit] 标签；
* 检测是否在 &lt;form&gt; 标签中使用了 id=”submit” 的标签；
* 检测是否将 &lt;style&gt; 块放置在 &lt;/head&gt; 前面；
* 检测是否将 &lt;script&gt; 块放置在 &lt;/body&gt; 前面；
* 检测&lt;img&gt;标签是否指定alt属性；
* 检测是否为input[text]指定label；
* 检测网页编码是否为gbk或utf-8；
* 检测是否使用了@import导入样式表；
* 如果CSS、JS指定 类似于“?t=20100405”时间戳，则自动输出最后修改时间，方便对比；
* 如果background-image超过6个，则提示所有背景图片及大小，超过30KB，标红显示；

### Monster评分规则：
Monster是根据问题解决难易程度、性能提升程度、可用性提升程度以及维护性提升程度来综合评分的。
具体请下载 [Monster评分算法.xls](https://github.com/alipay/monster/raw/master/Monster%E8%AF%84%E5%88%86%E7%AE%97%E6%B3%95.xls)

###### 这是Monster的第一版，欢迎抓虫，如果您有更好的改进建议，请反馈给我们。
