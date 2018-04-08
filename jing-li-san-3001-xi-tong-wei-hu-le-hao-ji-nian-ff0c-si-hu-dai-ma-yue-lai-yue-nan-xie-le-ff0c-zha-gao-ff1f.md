记得刚毕业的时候做的一地个稍微大点的需求。实际写的代码不超过100行，可是上线的时候还是挂了（知道出问题后，可提心吊胆了，觉得怎么能出这种错误呢，不是自认为还可以的吗。几年后回想：会觉得当时问题很low，而且有点不敢相信自己会犯这样的错误）。起始这个需求还是在老员工指导下完成的，就是东改改，西改改，然后就ok了。一上线，用户使用的时候发现不对，而后我就找出问题是需求时某一个点业务逻辑没有搞清楚，少了一个分支判断。

其实细想：现如今虽然软件开发人才需求量很大，岗位很多。但是多少还是以业务为主的，纯粹搞技术的公司相对比例还是比较少的（可能和个人的经历有关啊，这些并没有做调研统计，只是从招聘网站招聘公司以及周围的朋友就职情况看看）。所以很多时候你进入一个公司是维护已有的以业务为导向的系统，完全重头开始的新项目是比较少的。就我范的错误有如下几点值得注意：

* 理解业务很重要，特别是一些运行比较久的老系统。在你动手前最好是对公司业务，系统涉及的业务，系统的整体架构了解下（谁用你的系统，谁调用你的系统，你的系统又依赖调用了哪些组件，哪些系统）。如果你不大了解这些，可能是你每行代码都能看懂，可是这些代码组合起来你就是不知道他们是什么意思【这个时候整体的抽象理解比某个细节更重要哦】

* 代码质量  
  在我维护的那个系统，代码中某个文件已经有接近万行代码，在IDE打开文件，哗啦啦的向下拉个好多屏，看着都然让人头疼。

* 代码可测试性  
  同样是我接触的那个系统，打个包部署起来要接近5、6分钟，然后测试，永远无法在开发环境造出全流程的数据。进入测试环境测试的bug就可想而知了。开发也不愿意多测。其实我个人一直觉得开发应该是最会测试的\(虽然耗时，但是自己的代码怎么样测试自己应该是最清楚的\)。

鉴于上面代码质量，个人觉得如下的几个点有必要了解下：

1. 软件开发的原则（SOLID）  

2. 代码重构一二

3. 设计模式


