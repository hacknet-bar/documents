\(Written By Pitiedwzr,Err0r233\)

欢迎加入制作扩展的队伍中！首先，在阅读本指南之前，请将Hacknet与迷宫DLC通关一遍，并且有一定的英文基础（工地英语也行，谷歌翻译）。

讲在前面，关于Hacknet拓展的一些注意事项： 字库特别的少，一个鸽子的鸽都会显示成问号；Actions的部分flag未实装，我会在Actions章节讲解。

接下来看一个扩展的基本构成：

![](/resources/pic-extension/image1.png)

* Actions：触发
* Docs：文档（新闻，论坛等）
* Factions：等于Actions
* HackerScripts：黑客脚本（naix那种）
* Missions：任务
* Music：音乐
* Nodes：节点
* People：人口 用于AcademicDatabase 通用医疗
* Theme：主题
* Web：网页
* ExtensionInfo：扩展信息
* Intro：开始时的文字
* Logo：扩展标志
* WorkshopLogo：创意工坊相关，放到以后再讲

了解了这些之后，我们就可以开始制作扩展了。对于新人来说，我推荐使用官方提供的模板BlankExtension（你要是足够强 也可以自己写）找到blank（steamapps\/common\/Hacknet\/Extension）复制一份模板，并将文件名改成自己的扩展名。打开模板，把EDIT\_ME\_ExtensionInfo改为ExtensionInfo。打开它，会有这些东西：

![](/resources/pic-extension/image2.png)

![](/resources/pic-extension/image3.png)

* Name：扩展名称
* AllowSaves：是否自动保存
* StartingVisibleNodes：开始时显示的节点
* StartingMission：开始时的任务
* StartingActions：开始时启动的触发
* Description：介绍
* Faction：派系
* StartsWithTutorial：启动时是否有教程程序
* HasIntroStartup：在扩展开始时是否有文字
* StartingTheme：开始时的主题
* IntroStartupSong：扩展启动时的音乐
* SequencerTargetID：Sequencer的目标节点ID
* SequencerSpinUpTime：Sequencer预热时间（不确定）
* SequencerFlagRequiredForStart：Sequencer启动时必要的条件（感谢Err0r233的修正）
* ActionsToRunOnSequencerStart：Sequencer启动时的触发
* WorkshopDescription，WorkshopLanguage，WorkshopVisibility，WorkshopTags，WorkshopPreviewImagePath，WorkshopPublishID等都是与创意工坊有关的内容，后面再讲。

另外，我们还要增加一条设置语言的语句：
`<Language>zh-cn</Language>`


其他语言的设置：

![](/resources/pic-extension/image4.png)

当你将这些东西修改完成后，恭喜你！你已经向制作扩展迈出了第一步！不过，也不要太得意，因为这篇教程只是入门，离制作一个成功的扩展还差得很远。

