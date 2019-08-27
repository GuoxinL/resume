# 个人简历

## 个人资料
 - 刘国新/男/1993
 - 本科/东北农业大学成栋学院软件工程专业/2012-2016
 - 工作年限：3年
 - 期望职位：Java高级程序员
 - 期望薪资：面议
 - 期望城市：北京

##  联系方式
 - 手机：18612130100
 - Email：lgx31@sina.cn
  
## 工作经历
### 埃洛克航空科技（北京）有限公司
工作时间：2017.10~至今
担任职责：后端研发
#### 云匣子项目
技术点：_**MongoDB**_，_**MySQL**_，_**Redis**_，_**Spring Boot**_，_**Netty**_，_**MyBatis**_，_**Spring Cloud**_  
云匣子是一个给无人机提供定位追踪功能的模块，他可以以每秒一次的将当前无人机所在的位置（经纬度），海拔高度，航向角等相关数据发送到后端。
本人主要负责的工作是数据收集系统（Netty服务）的以及云匣子周边业务的开发，这个项目最大的难度是我在接手这个项目的时候前任的代码写的很差数据收
集系统耦合了大量的业务，我在保证数据收集系统稳定运行的情况下重构了该项目，拆分了业务和数据收集模块，解决了这个棘手的问题，后期在总结的过程中
抽象出面向业务的二进制流式通用传输协议（https://github.com/GuoxinL/protocol4java ）开源项目。

#### 中国空网空域地图服务项目
技术点：_**Geoserver**_，_**PostGis**_，_**WMS**_，_**JPA**_，_**AOP拦截请求/响应AES加解密**_，_**Spring Cloud**_  
本人主要负责地图服务的开发和维护，地图服务在空网后端的战略意义很大，地图服务负责空网三端（IOS，Android，PC）的地图显示，地图服务还负责保存
所有业务中的空域数据，支持业务区域校验，支持云匣子数据校验本人在负责整体项目的调研与架构，以及后期开发和维护，这个项目最大的难点是在于中期使
用过程中出现的坐标经度问题，因为对地理信息知识的不了解造成了坐标经度误差问题，后期在不断的测试和调研解决了坐标精度误差的问题

### 北京鑫丰南格科技有限公司
工作时间：2016.01~2017.10  
担任职责：后端研发，运维  

#### C系列项目（床头呼叫系统）
负责C系列（床头呼叫系统）的医护患模块和自动升级模块的开发和测试工作，在这个项目中最大的困难是整体项目在医院的运维工作，因为特定的环境下没有
外网情况下的Linux以及Windows运维难度很大，以及使用了微型服务器配合Clonezilla达到拆箱部署的方法，解决的系统的人肉运维，后期负责C系列的重
构以及将以往使用的Windows环境下部署迁移到Linux系统的部署工作。

#### 蜂鸟系列（医护患交互系统前身是床头呼叫系统）
技术点：_**MongoDB**_，_**MySQL**_，_**Redis**_，_**Spring Boot**_，_**Spring Data(Mongo,QueryDSL,Redis)**_，_**MyBatis**_，
_**ActiveMQ**_，_**OpenShip**_  
负责蜂鸟系列（医护患交互系统）的聊天模块，文章模块，科室模块，信息看板模块，文章模块，计费提醒模块，统一文件上传模块。
项目中的一部分与日志相关的数据业务存储在MongoDB中例如呼叫记录，还有一部分存储在MySQL中MySQL中存储主要业务模块，例如计费模块，文章模块，信
息看板模块等等，后端的框架主要使用的Spring Boot整合了Spring MVC，MyBatis，Spring Data(Mongo,QueryDSL,Redis)，使用Spring Boot 可
以快速方便的对项目的配置节省开发时间。  

项目的持续集成主要使用了Jenkins对前后端项目的代码进行一键的打包部署的自动化，减少了人肉运维的痛苦。
除了基本的代码工作在项目后期也担任项目的项目的运维工作，领导指示，要求把部署时间将到最短，达到让实施人员拿个U盘到某个医院在一天内就要将软硬
件快速的实施完成，在我这部分工作中主要是将部署实现自动化，编写了服务所依赖的数据库和中间件的自动安装脚本
（https://github.com/GuoxinL/installer ），以及Linux备份还原。  
参与服务器的选型和定制，服务器的系统使用Ubuntu-server 16.04.02。

在物联网的后端最大的问题一部分是数据收集系统的稳定性，还有一部分是对于传输协议的定义，市面上普遍的协议定义方式主要有（mqtt协议，二进制自定
协议）而公司内部使用的是二进制传输协议，在二进制协议定义的上面最普遍的做法是超前的预想业务和预留字段的方式，公司中有经验的
## 自我评价 

喜欢参加各种线下活动，在活动中学习了解学习新的技术交新朋友，喜欢打羽毛球，吊打产品（伪）^_^。
