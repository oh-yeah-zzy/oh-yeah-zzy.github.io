---
layout: archive
title: "研究项目介绍"
permalink: /research_project/
author_profile: true
---

## OCS项目介绍 {#ocs_research_project}

OCS的全称为observation control system/ observatory control system，两个不同的称呼代表了其不同的阶段，前者被称为观测控制系统，后者被称为台站控制系统。

前者在一定程度上可以被视为后者的子集，观测控制系统主要起到对观测流的控制作用，仅关注与观测流程相关的内容，而台站控制系统则在观测流的基础上，同步叠加对于台站其他设备状态的控制与关注，例如加入了故障诊断系统、观测策略系统等。

### 实验室自建小型望远镜观测控制系统

这台望远镜位于实验室楼顶，整体设备来源于以前的实验室项目，项目拆除后相关望远镜设备被运了回来，实验室将相关设备借了过来，搭建了可供实验室同学学习与使用的小型望远镜，非常不幸的是，在转移与重建的过程中，小型望远镜的镜筒受到了损坏，仅有支架与赤道仪等可用，实验室因此额外采购了一个非原装的镜筒，该镜筒与原装镜筒相比之下功能确有不足，例如只能手动调焦等等。

但是对于刚进入实验室的同学来说，该望远镜不失为一个非常好的练手选项，望远镜整体由支架、赤道仪、镜筒、相机、防水布、工控机及其外设、亚克力小房子组成，其他的部分均比较常规，均与正常的望远镜中该部分的setting相同，这里着重讲一讲与其他望远镜不大一样的部分：

+ **相机**：一般来说自己组装的望远镜相机会采用固定的，但是由于此望远镜为本实验室自建望远镜，而本实验室的另一大业务为相机研发，因此本望远镜所采用的相机并不固定型号，一般情况下回直接使用实验室空置的相机。
+ **亚克力小房子**：在望远镜的一般实践中，望远镜均会配备圆顶，起到为望远镜遮风挡雨的作用，但是由于经费的问题，我们并没有为该小望远镜采购/修建圆顶，而是使用了亚克力板与对应的结构骨架修建了一座小房子，该小房子底部采用福马轮支撑，在进行观测时仅需松开福马轮即可推开，露出望远镜进行观测。
+ **防水布**：这也是这个望远镜的特殊处之一，在一般实践中，仅依靠圆顶即可完成风雨的遮挡，但是由于亚克力板与结构骨架连接处存在缝隙，仅依靠亚克力小房子无法完成风雨的遮蔽，因为我们采购了防水布，在观测完成后会将防水布覆于望远镜上，防止风雨导致望远镜损坏，一种更好的实践是将防水布覆于亚克力小房子上，但是由于未能在实验室中找到如此巨大的防水布，我们并未采用此类实践。

搭建望远镜如下图所示：

<div style="text-align: center;">

<img src="/images/tel_upstairs_mor.jpg" alt="搭建完成的望远镜" width="50%">

<p>搭建完成的望远镜</p>

</div>

观测时我们需要将望远镜从小房子中推出来，推出来后的情况如下图所示：

<div style="text-align: center;">

<img src="/images/tel_upstairs1.jpg" alt="推出来观测的望远镜图1" width="50%">

<p>推出来观测的望远镜图1</p>

</div>


<div style="text-align: center;">

<img src="/images/tel_upstairs2.jpg" alt="推出来观测的望远镜图2" width="50%">

<p>推出来观测的望远镜图2</p>

</div>

我们一般会使用实验室空置的相机装在望远镜上来进行观测，相机安装后图像如下所示：

<div style="text-align: center;">

<img src="/images/455_upstairs.jpg" alt="安装好的相机" width="50%">

<p>安装好的相机</p>

</div>

该观测控制系统前后端整体采用了实验室传承下来的技术栈，前端采用了**vue2框架**，后端采用了**tornado+fastapi框架**，底层的分布式框架所使用的是**RACS2框架**，该控制系统主要由g哥搭建，是g哥的开山之作，g哥从此学会了如何使用RACS2框架进行开发，跨入了观测控制系统领域，笔者与实验室其他成员主要起到协助g哥，为g哥提供前后端开发修改支持/技术指导/bug修复/望远镜扛楼机的作用。

趣事杂记：

1. 在后续与g哥一起使用望远镜/修各种bug的过程中，我们有幸看到了可能/大概/或许是被台风摧毁的小棚子：

<div style="text-align: center;">

<img src="/images/tel_upstairs_break.jpg" alt="坏掉的亚克力小房子" width="50%">

<p>坏掉的亚克力小房子</p>

</div>

### 用于空间碎片观测的观测控制系统

实验室历史上其实接到过若干个用于空间碎片观测的观测控制系统的研发项目，笔者在写这里的时候思考了许久关于究竟该写哪一个空间碎片观测的项目，最终决定落笔写的这个项目，其所在的观测站址以及观测设备相较于其他的项目来说可能不是那么先进与昂贵，但是其具备着空间碎片观测最标准的设备，同时其具备着实验室历史上的OCS项目中**最标准**的控制接口以及**最高**的控制自由度。

由于空间碎片观测项目的特殊性，将与老师讨论后决定如何撰写该项目的描述。（该项目为g哥重点毕业项目，但是g哥的毕业论文目前我在知网上还搜不到，故此不是很敢写）

### WFST望远镜OCS

WFST望远镜是由中国科学技术大学与紫金山天文台共建的大视场巡天望远镜。其具备2.5m的主镜口径与3°的大视场，并具备多波段观测能力。其坐落于中国青海的冷湖台址，该台址气象条件良好，具备清晰良好的光度与视宁度条件，同时具有稳定的地面空气环境，是地球表面少数的几个高质量天文站点之一。

WFST望远镜本体具备2.5m的口径与3度的大视场，其科学成像部分使用了9片9k x 9k的传感器进行拼接，共计约700 million像素，同时，其主镜具备主动光学校正技术，能够有效改善像质，这也使得WFST具备非常强大的巡天能力，其巡天能力仅次于LSST，能够与LSST形成南北半球天区的互补。

该望远镜项目为实验室近几年来的主力项目，大部分同学的毕业论文与小论文均落在了该项目上，实验室主要参与了WFST望远镜的主焦相机与OCS部分的建设。

WFST OCS的主要目标是：

> The observatory control system (OCS) of WFST is structured based on the RACS2 framework, which is a low-level framework developed by our laboratory for the development of distributed control systems. It features decentralization and automatic component discovery. In this framework, components exist as nodes on a LAN message bus and communicate through the message bus. Additionally, the framework provides Python bindings, enabling users to rapidly develop components using Python.
> 
> During the observation period, the control of equipment requires accuracy, real-time, efficiency and safety. Therefore, we design and implement the OCS (observatory control system) of WFST which performs multi-layer abstraction on each hardware device and puts more attention on the operation of the observation process and the scheduling of observation tasks.

**以上目标引自部分已发表的论文。**

简单来说，WFST OCS的主要目标是完成WFST望远镜台站上各设备的控制，并在此基础上完成望远镜观测流的控制并在观测时尽可能地提高观测效率，增加单位时间内观测的天区面积，同时在观测时保障台站各设备的安全。

在该项目中，实验室的OCS完成了从观测控制系统阶段到台站控制系统阶段的跃迁，目前该项目正在台站控制系统的路上逐步地向前推进。不可否认的是，在推进的过程中，我们遇到了非常多的困难，在这里将部分困难罗列如下，或许我们能在不久的将来解决掉他们：

1. 底层框架的不足，在过去相当长的一段时间中，实验室所使用的分布式开发框架为RACS2框架，但是该框架在设计之初未能考虑到台站控制系统的需求，导致如果此时如果需要将所需特性添加到系统中会面临两方面的问题，一是若是通过节点的形式来添加，将导致框架外代码量过大，整个系统会呈现出一种尾大不掉的现象，二是如果修改底层代码以添加所需特性，由于原版的设计中并未考虑这些特性的添加，因此添加这些特性需要做大量底层代码的修改与测试，可能会导致整个系统的开发周期大大加长。
2. 整体系统的复杂性，前面提到了我们期望在系统中加入一些新特性，但是这些新特性由于底层框架的已有现状导致难以添加，而这些新特性的需求整体来讲是由于系统的复杂性导致的，由于台站设备的数量之众，观测时所需考虑的因素之多，台站设备权限的调度之困难，因此综合导致该OCS十分复杂。

需要强调的是，对于刚进入实验室的同学来说，该项目并不能说得上是一个非常好的练手项目，其设备与一般的望远镜系统不完全相同——许多设备与控制方式是WFST望远镜独有的，在一般的望远镜系统上并不具备，例如主动光学技术等等，为了能够使得望远镜达到国际先进水平，与主动光学技术类似的设计在WFST望远镜上还有许多。

趣事杂记：

1. 此事发生地点位于太站上。
    中午
    c哥：我刚上厕所被狗追了200m。
    笔者：哈哈哈哈哈哈哈哈。（内心OS：你看我信不信）
    晚上
    笔者：我刚上厕所被狗追了200m。
    c哥：哈哈哈哈哈哈哈哈哈。

<div style="text-align: center;">

<img src="/images/king_in_station.jpg" alt="台站的王" width="50%">

<p>台站的王</p>

</div>

## 相机项目介绍 {#camera_research_project}

### 相机测试平台项目

### 用于空间碎片观测的科学级相机研发

### 用于定位测量的CMOS相机研发

### 大靶面超高速率的sCMOS相机研发

### 顺手一块写了目前还不知道用于啥的sCMOS相机研发