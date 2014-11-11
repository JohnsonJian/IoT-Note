## 物联网工程概论

# 最后一节课的重点笔记
为了那些没去上课的同学准备

王与琛学神版权所有
<img src="http://zgqathit.qiniudn.com/IMG_1030.jpg" width=100%>



## 第一章

物联网关键技术与体系结构

## 第二章

RFID全部内容

## 第三章

无线传感器网络，智能传感器

## 第四章

智能系统核心 穿戴和智能机器人 P143

## 第五章 （基本不考）

接入技术 6lowpan

## 第七章

重点

## 第八章

数据融合 云计算 数据挖掘

## 第九章

安全防护 体系结构 攻防类型

## 第十章

（基本不考）对设计题有帮助

<hr>

## 知识点总结（考不考就不知道了）

### 第一章 物联网概述

1. 物联网的主要特征是：全面感知，可靠传输，智能处理
2. 物联网的主要技术特征
   
   1. 物联网智能物体具有感知，通信和计算能力
   
       （1）“智能物体”是对连接到物联网中的人和物的一种抽象
       （2）对“智能物体具有感知，通信和计算能力”的理解
            
            1. 智能物体的生物特征可能不一样，但是都具有感知，通信和计算能力
            2. 智能物体能感知到那些参数,与所选用的传感器或RFID类型有关。
            3. 通信能力的不同表现在：它可以主动发送数据，也可以被动发送数据；可以使用有线方式通信，也可以使用无线方式通信；可以使用微波信道通信，也可以用红外信道通信；
            4. 计算能力的不同表现在：它可能只是简单的产生数据，可能是进行计算量较小的数据汇聚计算，也可能进行计算量较大的数据融合，路由选择，拓扑控制，数据加密和解密，身份认证计算与控制。

        （3）对物联网标示符的理解
        
            物联网中的RFID标签目前影响最大的两个标准——电子产品编码（EPC）与泛在识别（UID）标准
            
        （4）智能物体与嵌入式技术的关系
            
            智能物体都应该是一种嵌入式电子设备，或者是装备有嵌入式电子设备的人，动物或物体。
            
    2. 物联网可以提供所有对象在任何时间、任何地点的互联
    3. 物联网的目标是实现物理世界到信息世界的融合

3. 物联网层次结构模型

        (1) 应用接口层
        (2) 智能处理层
        (3) 网络传输层
        (4) 物联接入层
        (5) 信息感知层
4. 物联网层次结构模型的另一种说法
	1. 感知层
	2. 网络层
	    1. 接入层
	    2. 汇聚层
	    3. 核心交换层
	3. 应用层
	    1. 管理服务层
	    2. 行业应用层
        
        
        
### 第二章 RFID与物联网应用

1. 条形码技术

    1. 一维条形码 
        
        优点：编码规则简单，条形码识读器造价较低
        
        缺点：尺寸大，空间利用率低，一旦损坏将出现拒读
        
    2. 二维条形码

        优点：信息容量大，译码可靠性高，纠错能力强，制作成本低，保密和防伪性能好
        
 2. 磁卡与IC卡
     
     IC卡也叫智能卡，它是通过在集成电路芯片中写有数据来识别的
     
 3. RFID基础知识
 
     1. RFID基本概念
         
         RFID利用无线射频信号空间耦合的方式，实现无接触的标签信息自动传输与识别技术。RFID标签又称为“电子标签”，或“射频标签”。
         
     2. RFID基本工作原理
         
         (1) 被动式RFID标签工作原理
         
                 读写器向标签传递能量，标签向读写器发送标签信息的过程。
                 读写器与标签之间能够双向通信的距离称为“可读范围”，或“作用范围”。
                 
                 
         (2) 主动式RFID标签工作原理
         
                 也称为有源RFID标签，由内部配置的电池供电。有源标签工作的过程中就是读写器向标签发送读写指令，标签想读写器发送标识信息的过程。
                 
         (3) 半主动RFID标签
         
                只有在读写器访问时，内置电池向RFID芯片供电，以增加标签的读写距离，提高通信的可靠性
                
      3. RFID标签的分类

         (1) 按供电方式分：无源标签和有源标签
         (2) 按工作模式分：主动式，被动式，半主动式
         (3) 按读写方式分：只读式和读写式
         (4) 按工作频率分：低频，中高频，超高频，微波段
         (5) 按封装材料分：纸质，塑料，玻璃
         
      4. RFID读写器
          
         主要功能有：与RFID标签通信，与计算机通信，对多个标签同时读写，能够纠错，能够识别有源RFID标签与电池相关的电量信息
         
         (1) 读写器的分类
                 
                 1. 移动式读写器
                 2. 固定式读写器

      5. RFID标签编码标准

         (1) EPC Global RFID标准
             
                 1. 为每一个产品分配一个唯一的电子标识符——EPC码
             
                 2. EPC码存储在RFID标签的芯片中

                 3. 对象名字服务 ONS(类似DNS）

         (2) UID编码体系
         
         (3) ISO/IEC RFID标准体系
             
      
             
                
### 第三章 传感器，传感网与无线传感器网络技术

1. 传感器概述

    1. 传感器的基本概念
    
        传感器是有敏感元件和转换元件组成的一种检测装置，能将检测和感受到的信息，按一定规律变换成电信号（电压，电流，频率或相位）输出，以满足感知信息的传输，处理、存储、显示、记录和控制的要求。
        
        
    2. 传感器的分类

    
       物理传感器：力传感器，热传感器，声传感器，光传感器，电传感器，磁传感器与射线传感器
       
       化学传感器：按传感方式分：接触式，非接触式；按结构形式分：分离式，组装一体式；按检测对象分：气体，离子，温度
       
       生物传感器：...
       
    3. 传感器性能指标

        精确度，分辨率，灵敏度，漂移，测量范围，精度，迟滞，线性度，噪声
            
    4. 执行器
    
        电子，液压，气动
        
    5. 智能传感器
    
    	 有内存和处理器，与数据网络进行交互
    	 
        智能传感器特点：1.自学习，自诊断和自补偿能力；2.复合感知能力；3.灵活的通信能力
        
 2. 无线传感器网络

     无线分组网（Ad-hoc网络） -> 无线传感器网络（WSN)
     
     无线传感网网络特点
     
     1. 网络规模大
     2. 自组织网络
     3. 拓扑结构的动态变化
     4. 以数据为中心

     无线传感网网络节点类型：
     
     1. 传感器节点
     2. 汇聚节点
     3. 管理节点
     
     
### 第四章 物联网智能设备

1. 嵌入式系统
    
    1. PC -> PDA -> GPS接收器 -> 智能手机 -> 智能家电 -> 数字标牌
    
    2. 智能传感器的重要基础之一是嵌入式系统
    
2. RFID读写器与中间件软件设计
	
3. 无线传感器网络节点设计 

	1. 无线传感器网络节点设计原则
	     
	     * 微型化与低成本
	     * 低功耗
	     * 灵活性与可扩展性
	     * 鲁棒性

4. 可穿戴计算

    1. 新的人际交互模式
         
         * 持久性
         * 增强性
         * 介入性
        
     2. 六个属性
         
         * 非限制性
         * 非独占性
         * 可觉察性
         * 可控性
         * 环境感知性
         * 交流性
         
     3. 三大能力
     
         * 移动计算能力
         * 智能助手能力
         * 多种控制能力
         
         
 5. 智能机器人
  
        * 工业机器人
        * 农业机器人
        * 服务机器人
        * 医用机器人
        * 微机器人与微操作机器人
        * 特种机器人
        * 军用机器人

### 第五章 计算机网络与互联网技术的发展

1. 接入技术
	
	* 有线接入
		* 电话交换网接入
		* 有线电视网接入
		* 光纤接入
		* 局域网接入
		* 电力线接入
	* 无线接入
	   * 无线局域网接入
	   * 无线自组网接入
	   * 无线城域网接入
	   * 移动通信网接入

2. ZigBee/IEEE 802.15.4
3. 6LoWPAN

### 第七章 位置信息、定位技术与位置服务

1. 位置信息与位置服务

   1. 位置信息在物联网中的作用
  		
  		* *位置信息*是各种物联网应用系统能够实现服务功能的基础
  		* 位置信息涵盖了空间、时间与对象三要素
     
   2. 物联网中的位置服务

   		* 基于位置的服务（LBS）
   		* 位置服务两大功能：确定位置，根据位置提供适合的服务

   3. 定位系统

  		* 数字地球——遥感（RS)，全球定位系统（GPS），地理信息系统（GIS），互联网地图
  		
  		
  	   GPS系统：
  	   * 提供导航，定位，授时等服务
  	   * 全球主要GPS系统：美国GNSS，欧盟“伽利略”，俄罗斯“格洛纳斯”，中国“北斗”
  	   * GPS组成：空间部分，地面控制部分，用户终端
  	   
 
### 第八章 物联网数据处理技术

1. 物联网数据的特点
    
* 海量
* 多态
* 动态
* 关联

2. 物联网数据处理关键技术

* 海量数据存储
	
	* TinyDB
	* IDC（互联网数据中心）
	* 云计算的特点：弹性服务，资源池化，按需服务，服务可计费，泛在接入）
	* 云计算数据中心的特点：自治性，规模经济，规模可扩展）
	* IaaS,PaaS,SaaS
	* 物联网数据中心的特征：部署快捷，运行可靠，可扩展，安全，节能
	
* 数据融合
   
   * 利用节点的本地计算与存储能力处理数据的融合以除去冗余信息
   * 根据融合前后信息含量分类：无损失融合，有损失融合
   * 根据与应用层数据语义之间关系融合：依赖于应用的数据融合（ADDA），独立于应用的数据融合（AIDA），两种技术结合的数据融合
   * 根据融合操作基本分类：数据级融合，特征级融合，决策级融合
  
* 数据查询、搜索和数据挖掘
  
   * 数据挖掘：在大型数据库中发现，提取隐藏的预言性知识的方法
   * 使用统计方法和人工智能方法找出普通数据查询中所忽视的数据隐含的趋势性的信息
   * 有效地利用物联网的海量数据已经成为物联网应用的关键，而数据挖掘技术对于物联网实现智能处理至关重要。


### 第九章 物联网信息安全技术

1. 物联网攻击手段

   * 欺骗类攻击
   * 拒绝服务攻击与分布式拒绝服务攻击
   * 信息收集类攻击
   * 漏洞类攻击

2. 物联网安全防护技术

   * 防火墙
   * 入侵检测与防护
   * 安全审计与取证
   * 网络防病毒
   * 业务持续性规划
  

3. RFID攻击方法

   * 窃听与跟踪攻击
   * 中间人攻击
   * 欺骗，重放与克隆攻击
   * 破解与篡改攻击
   * 干扰与拒绝服务攻击
   * 灭活标签攻击
   * 病毒攻击
  
 
   

### 第十章 物联网应用
