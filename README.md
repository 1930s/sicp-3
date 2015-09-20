## SICP

[![SICP](http://img4.douban.com/lpic/s1113106.jpg)](http://www.sicp.pub/)

[SICP](http://book.douban.com/subject/1451622/)，一本讲解编程真谛的经典教材。之前上大学期间，陆陆续续看了2遍这本书，无奈都没坚持到底。第一次只看完第一章，第二次只看完前三章。很多习题也没做。

这，是第三次进攻。这个repo会记录我在看SICP时的习题代码与一些自己的笔记与想法，这么做一方面是给自己查漏补缺，另一方面也为希望对今后阅读sicp的人有些许帮助。

## Why SICP 

- [老赵书托（2）：计算机程序的构造与解释](http://blog.zhaojie.me/2009/07/recommended-reading-2-sicp.html)  
- [向热爱计算机科学的你推荐SICP](http://www.nowamagic.net/librarys/veda/detail/1905)
- 王垠的[如何掌握程序语言](http://yinwang0.lofter.com/post/183ec2_47bea8)

##目标

在**2016年1月1号**之前啃完**所有章节与习题**！！

## 环境准备

工欲善其事必先利其器。下面说下我Mac上的scheme环境：

- ![Mac 环境](mac-env.png)
- [mit-scheme 9.2](http://ftp.gnu.org/gnu/mit-scheme/stable.pkg/9.2/mit-scheme-9.2-x86-64.dmg)，我的Mac版本是10.10.2，按照上这个官方scheme后点击图标，闪退，不清楚为什么，我这里直接把`MIT:GNU Scheme.app/Contents`下的`Resources`文件夹拷贝出来，并把它加入的PATH中，这样就能够运行了。
![mit-scheme screencast](http://ww2.sinaimg.cn/mw690/5fee18eegw1es79f0y9u2j21tm0eqjus.jpg)
- 这里安装好的scheme在交互式环境下[无法使用方向键](http://stackoverflow.com/questions/27648559/mit-scheme-cant-move-left-when-enter-code)，可以通过安装rlwrap解决（`brew install rlwrap`）之后，用`rlwrap mit-scheme`启动就可以了。
- 英文版epub＋中文版实体书，计算机的书最好还是看英文原版，我这里买了中文版的实体书，英文版的好贵！<del>不过[多看](http://duokan.com/)对epub格式支持很好，放手机上看很方便，而且多看支持划词翻译，写笔记，笔记同步Evernote等等，真是太方便了，推荐大家使用。</del>手机屏幕还是太小了，而且很容易分心，[Kindle Paperwhite](http://www.amazon.cn/gp/product/B00QJDOLIO)才是真爱，值得拥有💖。
- mit-scheme直接从文件中读取代码并执行，例如有个文件名为`fib.scm`的文件，在scheme交互式环境下通过`(load "fib.scm")`命令就能够执行`fib.scm`中的代码了。
- 2.2.4小节用到的图形语言采用Racket实现，这是它的[文档](http://planet.racket-lang.org/package-source/soegaard/sicp.plt/2/1/planet-docs/sicp-manual/index.html)。
- 2.4.3小节`put`与`get`的实现，参考[/exercises/02/lib/hash_table.scm](/exercises/02/lib/hash_table.scm)

我的初始化环境就是这样了，后面如果有改变我会修改这里的说明。

## 一些资料

- 首先是[MIT的视频公开课](http://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-001-structure-and-interpretation-of-computer-programs-spring-2005/video-lectures/)，为了方面观看，我写了个脚本把这些视频＋英文字幕下来了，并且传到了[百度网盘](http://pan.baidu.com/s/1jGrI5EY)上，有需要的可以自取。
- [SICP书中的源码](http://mitpress.mit.edu/sicp/code/index.html)
- [epub格式的英文原版 + 在线HTML5版sicp](https://github.com/sarabander/sicp)
- [北大SICP教学主页](http://www.math.pku.edu.cn/teachers/qiuzy/progtech/)，强烈推荐，课堂PPT总结的很好，还有中文版的[勘误表](http://www.math.pku.edu.cn/teachers/qiuzy/books/sicp/errata.htm)。

## 战友

很有幸，这次我不是一个人。我和三个同事成立了个sicp学习小组，相互督促，相互交流。经过两周的试验，发现效果还比较满意。

感谢你们，希望能够一起享受这一次奇妙之旅。

- [南瓜](https://github.com/ng-wei)
- [耗子](https://github.com/haozi-yz)
- [小挖](https://github.com/jerrychen1990)

如果你有兴趣，欢迎加入我们的SICP读书QQ群：`119845407`。（手机QQ可直接扫码😊）

![](SICP_QQ.png)

## Timeline

- 2015-5-17  第三次开启SICP之旅
- 2015-7-12  结束第一章，构造过程抽象。[我的总结](http://liujiacai.net/blog/2015/07/18/sicp-chapter1-summary/)
- 2015-9-20  结束第二章，构造数据抽象。[我的总结](http://liujiacai.net/blog/2015/09/20/sicp-chapter2-summary/)
