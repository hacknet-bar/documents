# 1.	Web
Web是一个网页服务器的储存资料文件夹…

比如Hacknet中的Nortron网页服务器的源码就储存在那

如果你有HTML的基础是可以轻轻松松编写一个web的

但作者太垃圾了，不会写

所以我就直接搬了…

Hacknet web资源都在`steam\steamapps\common\Hacknet\Content
`的Web文件夹中，如果是html的大佬可以自己查阅

本萌新在此不过多展开

# 2.	People
People，也就是人口，在Hacknet中虚构的人口。

比如CSEC中的叫你删除
学位的那个人就是一个虚构人物

那么我们要怎么才能创建出一个People呢？

1. 在ExtensionsInfo同目录文件夹下创建People文件夹（若已经有，可以省略这一步）
2. 从IntroExtension复制模板（ExamplePeople.xml）然后打开

_题外话：我的导师Forever_天蓝说过 IntroExtension是一本百科全书_

_有什么事都可以去查阅它，所以我希望大家能够善用IntroExtension
_
 
第三步，编辑
如果你已经成功打开ExamplePeople.xml 你应该可以看到上图界面

<Person id="personID" handle="tester" firstName="Joe" lastName="Citizen" isMale="true" forceHasNeopals="true">
这是这个人的基本信息：
Person id: 这个人的代号 其实是方便编辑者编辑的
Handle: 不知道如何翻译，亲测只需跟PersonID一样即可
First name和last name不必解释
IsMale：是否是男性
ForceHasNeopals: 是否有Neopals的点数

<Birthplace name="Califonia" />

出生地名字：加利福尼亚
可以改成自己想要的，甚至可以打Unknown

<Degrees>
    <Degree uni="University of California" gpa="3.2">Bachelor of Software Engineering</Degree>
    <Degree uni="University of California" gpa="3.4">Bachelor of Business Management</Degree>
  </Degrees>

Degrees: 学历 一个人可以拥有多个学历
gpa：就是点数… 可以随便改

<Medical>
    <Blood>AA</Blood>
    <Height>178</Height> 
    <Allergies>Commas,Separate,Allergies</Allergies>
    <Perscription>Spironolactone x70 bi-monthly :: Aldosterone Inhibitor as a cardiac regulator</Perscription>
    <Perscription>You can write whatever you want here!</Perscription>
    
    <Notes>These notes show up in the medical record too. You can include IP addresses and passwords etc here if you want.</Notes>
  </Medical>

上面是用于通用医疗数据库的关于医疗的信息

Blood：血型
Height：身高 单位：cm
Allergies：过敏症…?
Perscription：处方 随便写就完事了
Notes：医疗记录

<DOB>17/02/1990 09:00:00</DOB>

出生时间，用于通用医疗数据库

<Notes>These notes are never used in-game, but can be handy to keep track of stuff for your own purposes.</Notes>
在/Medical下面的笔记是永远不会出现在游戏中的
打笔记专用…

