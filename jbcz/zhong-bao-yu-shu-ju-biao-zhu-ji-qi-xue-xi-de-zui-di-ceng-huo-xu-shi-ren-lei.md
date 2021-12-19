# 众包与数据标注：机器学习的最底层，或许是人类

**众包与数据标注：机器学习的最底层，或许是人类**

“人工智能正在广泛地取代传统劳动力，然而，从某种意义上来说，机器学习的发展，也创造出了更多岗位，和更多谋生的可能。人类并非直接服务于人类，而是被用于「训练机器」。”

***

现在，更多的科幻作品将目光着眼于机器对人类造成的威胁，警惕于人工智能的迅速发展。机器通过了「图灵测试」，亦或是违反了「阿西莫夫三定律」—— 许多科幻故事就由此开始。

![img](https://jibencaozuo.com/static/media/01.cd95271b.gif)

《爱，死亡，与机器人》第一季

除了可能的肉体伤害 —— 比如你会在电影《我，机器人》中见到的那样，**越来越聪明能干的机器，也暗暗推动了人类的内卷。**

随着机器大规模地取代人类劳动者，就业率的增长不再与经济增速保持同步。2016 年，富士康工厂用机器人取代了 6 万名工人，而亚马逊则在 20 个物流中心部署了 4.5 万台机器人。这些数据证明了人工智能发展对蓝领制造业的巨大冲击，也似乎佐证了那句「内卷名言」：不抓紧时间努力的话，你的工作就要被机器抢走了。

然而，**从某种意义上来说，机器学习的发展，也创造出了更多岗位，和更多谋生的可能。**

这其中当然包括电子元件生产商、电脑维修店老板，或者你的编程课老师，但还有一些人，他们并非直接服务于人类，而是被用来训练机器。

#### 机器学习的「练习题」，越多越好

人类收集、标注海量数据，再将数据输入机器训练模型，让机器根据输出结果与正确答案间的差值，进行反复迭代和修正，这就是现在常用的机器学习形式之一，**监督式学习**。

在基本操作的交互视频课程\*\*《一个人工智能的诞生》\*\*EP 01「识别数字」中，有一个监督式学习的典型例子。为了训练出一个可以识别数字 3 或 7 的神经网络，我们需要先把 12396 张预先已经被标记为 3 或 7 的图片输入电脑。

![img](https://jibencaozuo.com/static/media/02.1cf3283e.gif)

这 6131 张数字 3 和 6265 张数字 7，全部来自一个叫做 MNIST 的数据库。整个数据库中共有七万张被标注好的手写数字的图片，并且被处理为统一的质量和大小，可以很方便地用于训练机器的图像识别能力。

这七万张图片来自哪里？

![img](https://jibencaozuo.com/static/media/03.7b186f6a.gif)

根据 MNIST 网站上的说明，库中的所有手写数据都来自美国国家标准技术研究所（NIST）的特殊数据库 3 和特殊数据库 1 。前者中的数字由人口调查局的雇员书写，后者则来自高中学生 —— 他们可以被视为有组织的兼职劳动者或志愿者（取决于他们是否得到报酬），背景和特质也较为统一。

然而，如果我们希望自己训练出的机器学习模型可以在更广阔的范围内识别手写数字，就需要为机器提供更多且更多样的「练习题」，毕竟，即便是在世界范围内已经相对统一的阿拉伯数字，也有太多种不同的写法。

![img](https://jibencaozuo.com/static/media/04.d149bd17.png)

德国人习惯的阿拉伯数字写法。| Osterhase on Ublog

那么，如何让更多地方、更多年龄的人，为数据库书写数字？或者，更广义地说，**如何让机器得到更丰富多样的训练素材？**

#### 任何时间，任何地点，他们为机器工作

如同上文提到的两个 NIST 特殊数据库，在过去，企业通常通过短期雇佣或者外包的方式，为某个需要大量样本的项目找到尽可能多的劳动者（非营利组织则可能主要依赖志愿者）。**而在今天这个「万物互联」的时代，随时调用不同地区、不同背景的人力资源，已经不再困难。**

需要以 70 多种语言向全球用户提供数字产品与服务的微软，创立了在线平台 Universal Human Relevance System（UHRS），微软的全职雇员以及授权合作伙伴可以在 UHRS 上提交申请，按需招募来自世界各地的工人，负责检查录音、核对文本、翻译、市场调查等基础工作。不需要到岗上班，工人们在家中就可以通过网络寻找并完成任务，按单获取酬劳。**这种依赖网络与自由劳动力的人力资源雇佣模式，被称为「众包（crowdsourcing）」**。

相比于传统的外包（outsourcing）模式，雇主可通过众包雇佣到的劳动力群体更加多样，价格也更低廉 —— 据研究员帕诺斯・伊佩罗提斯估计，在亚马逊旗下的众包网站 Amazon Mechanical Turk （AMT）上，任何时候都有 2000 至 5000 名工人在准备工作，而 AMT 为每项工作设定的最低报酬仅为 1 美分。显然，这种雇佣模式非常适合用于高效训练人工智能，以至于直接被作为样例写在了 AMT 网站的首页上。

国内的情况也很类似。随着人工智能产业在国内的迅速发展，大大小小的数据标注平台也在为飞速增长的数据训练需求服务。规模较小的数据标注企业仍然以传统的雇佣关系为主，而在百度众包、京东众智等较大的数据服务供给平台，其人力构成的基本结构，是少量的数据专家、正式雇用职工，和大量通过众包平台招募的临时工人。

![img](https://jibencaozuo.com/static/media/05.da080481.png)

百度智能云在 2000 多名正式标注人员外，还有 10 万以上的外部标注人力。| 百度智能云宣传片

而这类工作的酬劳，和标注数据的难易程度直接挂钩。数据标注的定价主要参考两个因素：标注时间和判断时间。简单来说，前者指标注方式，比如2D拉框或者语义分割，后者则主要指需要标注的元素是否容易识别。对于未经专业培训的众包工人来说，能够被分配到的任务通常较为简易，因而酬劳也更低。如识别数字这类任务的售价，可能仅为 0.004 元/次，工人从中得到的酬劳必然更低。要想赚到一杯 20 元的奶茶钱，你可能需要完成超过 5000 次数字识别，还要保证自己在这样的机械劳动中，不会因为疲劳和肌肉惯性产生判断错误。

#### 带薪看 R 级片，也许并不美好

或许你听过那个有关自动存取款机的段子：你放进去的纸币之所以能被准确无误地数出来，是因为真的有银行柜员躲在 ATM 里上班。同样，在那些需要你通过标记图像来证明自己并非机器人的网站上，也是真正的人类，预先圈出了图中所有的公交车、自行车，或者交通灯，以此告知机器，「能在这个地方按下鼠标的，就可以被判定为人类。」

![img](https://jibencaozuo.com/static/media/06.94a0c71d.png)

也有文章认为，你对这些图片的辨别，

实际上是在为谷歌的无人驾驶技术服务。

正如《一个人工智能的诞生》EP 12中提到的，机器擅长的是有明确规则的事情，但我们无法总结出几条确定的规则，告诉机器到底什么是消防栓，什么是红绿灯。在今天，人工智能已经发展到前所未有的高度，却仍然无法对一些人类可以轻易回答的问题作出迅速判断，特别是在涉及情感和主观判断的部分。**一个典型的例子，就是内容审核。**

对不同认知背景的人来说，同样的词语或图像可能具有多种不同的含义，最为典型的就是「呵呵」和社交网站上的「微笑」表情。\*\*更复杂的情况，则出现在以用户上传的信息为主的网站上（即 UGC 网站，user-generate-content），特别是近年来兴起的直播。\*\*相比静态的图片和文字，或者可预先审查的录播视频，直播中的内容更加无法预测，上一秒还在吃喝玩乐的主播，下一秒可能就会做出一些极端行为。

正如《一个人工智能的诞生》中提到的，机器学习的最底层是数学。尽管人工智能科学家们在尽可能地使自己的机器训练模型适应更多的应用场景，但**在某些难以用数字量化的领域，人类的判断作为对机器识别的补充，仍然不可或缺。**

![img](https://jibencaozuo.com/static/media/07.e6e83141.png)

正在进行的数据标注：人脸关键点定位 | 当下频道

在处理来自用户的举报之外，视频网站审核的常见模式，是先通过机器对视频进行图片抽帧分析，判断截图中是否包含高风险内容，而机器无法直接判断的，则会被送到人工审核员的屏幕上，进行二次分析。在瞬息万变的直播中，显然很容易存在「漏网之鱼」。在 2017 年的一次直播杀人事件之后，Facebook 增加了 3000 名人工审核员，专门审查暴力直播视频。可见，**对于巨大的 UGC 市场来说，人工智能还不能完全取代人类。**

![img](https://jibencaozuo.com/static/media/08.cf1f2ed1.jpg)

一部反映网络审查员生存状况的纪录片《网络审查员》| 豆瓣电影

既然人工判断在内容审核中如此必要，**从事这类工作的人处境如何？**

和大多数工种相比，网络内容审核员们需要长时间直面更密集、更暴力的文字、图片或视频信息，并被要求在短时间内作出判断，因此\*\*更容易患上创伤后应激障碍，也无法保证正常作息，健康状况面临着更严峻的威胁。\*\*此外，大多数审核员都来自外包公司，与互联网巨头的正式员工们有着巨大的待遇鸿沟，更何况，更多的自由职业者正在通过众包平台加入其中。缺乏组织保护，又处在众包体系的权利最底层（无法得知雇主信息、无法得知项目目的、没有保险等），使他们的人身权益更难得到保障。很多时候，众包劳动者们只能依靠自建的论坛、社群来分享信息，相互鼓励，为彼此提供帮助。

毫无疑问，机器正在变得更加聪明，但与之相对的，人类也期待着人工智能在更多领域内的应用，自动化的终点永远都在改变 —— 这被称为\*\*「自动化的最后一英里悖论」\*\*，沉重地压在这些为机器工作的劳动者肩上。

在可以预见的近未来，人类与机器相互协作的模式，还将长久地持续下去，而在享受机器学习带来的便利的同时，我们也应该看见那些机器的「陪练员」们，和他们所面临的身心问题。**这种新型工作模式，看似为人们提供了更多自由，但一旦被困入其中，所谓的「选择」，或许只是假象。**

\*\*题图：\*\*Levi Stute on Unsplash

**参考资料：**

(1) **玛丽·L.格雷,西达尔特·苏里. (2020).** 销声匿迹：数字化工作的真正未来. 上海: 上海人民出版社

(2) **H. Reese, Heath. N. (2016).** INSIDEAMAZON'S CLICKWORKER PLATFORM:How half a million people are being paid penniesto train AI. TechRepublic.

(3) **李婷(编). (2014).** 人与机器共同进化. 北京: 电子工业出版社

(4) **光谱. (2020).** 独家"内部员工揭秘：TikTok 竟然这么审核内容. 品玩. https://www.pingwest.com/a/212302

(5) **36氪. (2020).** 互联网内容审核员，机器背后的"打工人". 新浪科技. https://tech.sina.com.cn/i/2020-12-25/doc-iiznezxs8883611.shtml

(6) **赵子潇. (2020).** Facebook 审核人员暴增，科技巨头的漫漫审核路. 极客公园. https://www.geekpark.net/news/258377

(7) **biu. (2020).** 大家好，我们是社交网络审核员. 极客公园. https://www.geekpark.net/news/261233

(8) **刘子珩.** **(2018).** 离职内容审核员的口述："我把内容扒给你看". 艾瑞网. http://column.iresearch.cn/b/201809/844468.shtml

(9) **冯颖星. (2021).** 我，鉴黄师，做审核生意年入几千万丨后窗. 投中网. https://www.chinaventure.com.cn/news/78-20210404-361353.html

(10) \*\*腾讯科技. (2019).\*\*调查称Facebook内容审核员薪水低、压力大到想自杀. 腾讯科技. https://tech.qq.com/a/20190226/002661.htm

(11) **勿忘初心. (2018).** 内容审核向左，还是向右？. 网易数帆. https://sq.163yun.com/blog/article/222859293683503104

(12) **apophisTech. (2018).** 讲真，Google欠你一辆车 你真以为是在输入验证码？. 腾讯云.https://cloud.tencent.com/developer/news/371927

(13) **当下频道. (2019).** 我成了人工智能里的人工，时薪五分钱 " 当下乱码S1E9. Bilibili. https://www.bilibili.com/video/av40256209

(14) **觉醒向量AWK. (2019).** 如何运营一家数据标注公司（参考报价篇）. 知乎. https://zhuanlan.zhihu.com/p/83477858

(15) **甲子光年.** **(2018).** “数据折叠”：人工智能背后的人工. 知乎. https://zhuanlan.zhihu.com/p/33955623