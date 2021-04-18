# 个人简历

## 个人资料
 - 刘国新/男/1993
 - 本科/东北农业大学成栋学院软件工程专业/2012-2016
 - 工作年限：4年
 - 期望职位：Golang开发工程师
 - 期望薪资：面议
 - 期望城市：北京

##  联系方式
 - 手机：18612130100
 - Email：lgx31@sina.cn

## 工作经历
### 易鑫集团

工作时间：2019.9~至今
担任职责：风控研发工程师

##### 风控项目-模型特征服务

技术点：**Golang**，**MySql**，**Redis**，**实时计算**，**并发**

易鑫主要业务是买车贷款业务，其中风控项目主要是针对个人的风险评估，为算法组训练的模型提供特征配置平台，在特征服务中将上千特征的取值运算返回给上层服务，其中有许多的难点，例如基础方法拓展，取数逻辑公式化，通过可配置的方式快速开发特征，供模型上线；在技术选型时考虑到用Python作为Web服务提供接口时会有性能瓶颈，所以使用Golang作为后端语言，实现模型加载，特征处理，映射，WOE，处理数据等周边服务；在开发过程中抽象不同层面的通用组件(https://github.com/GuoxinL/gcomponent)，并对性能进行优化（pprof）并积极探索新的技术。

### 埃洛克航空科技（北京）有限公司

工作时间：2017.2~2019.9
担任职责：后端研发

##### 云匣子项目

技术点：_**MongoDB**_，_**MySQL**_，_**Redis**_，_**Spring Boot**_，_**Netty**_，_**MyBatis**_，_**Spring Cloud**_  
云匣子是一个给无人机提供定位追踪功能的模块，他可以以每秒一次的将当前无人机所在的位置（经纬度），海拔高度，航向角等相关数据发送到后端。本人主要负责的工作是数据收集系统（Netty服务）的以及云匣子周边业务的开发，这个项目最大的难度是我在接手这个项目的时候前任的代码写的很差数据收集系统耦合了大量的业务，我在保证数据收集系统稳定运行的情况下重构了该项目，拆分了业务和数据收集模块，解决了这个棘手的问题，后期在总结的过程中抽象出面向业务的二进制自描述通用传输协议（https://github.com/GuoxinL/protocol4java ）开源项目。



##### 中国空网空域地图服务项目
技术点：_**Geoserver**_，_**PostGis**_，_**WMS**_，_**JPA**_，_**Spring Cloud**_  
本人主要负责地图服务的开发和维护，地图服务在空网后端的战略意义很大，地图服务负责空网三端（IOS，Android，PC）的地图显示，地图服务还负责保存所有业务中的空域数据，支持业务区域校验，支持云匣子数据校验本人在负责整体项目的调研与架构，以及后期开发和维护，这个项目最大的难点是在于中期使用过程中出现的坐标经度问题，因为对地理信息知识的不了解造成了坐标经度误差问题，后期在不断的测试和调研解决了坐标精度误差的问题。

### 北京鑫丰南格科技有限公司
工作时间：2016.01~2017.2
担任职责：后端研发，运维  

##### C系列项目
负责C系列的医护患模块和自动升级模块的开发和测试工作，在这个项目中最大的困难是整体项目在医院的运维工作，因为特定的环境下没有外网情况下的Linux以及Windows运维难度很大，以及使用了微型服务器配合Clonezilla达到拆箱部署的方法，解决的系统的人肉运维，后期负责C系列的重构以及将以往使用的Windows环境下部署迁移到Linux系统的部署工作。

##### 蜂鸟系列
技术点：_**MongoDB**_，_**MySQL**_，_**Redis**_，_**Spring Boot**_，_**Spring Data(Mongo,QueryDSL,Redis)**_，_**MyBatis**_，_**ActiveMQ**_，_**OpenShip**_  
负责蜂鸟系列的聊天模块，文章模块，科室模块，信息看板模块，文章模块，计费提醒模块，统一文件上传模块。项目中的一部分与日志相关的数据业务存储在MongoDB中例如呼叫记录，还有一部分存储在MySQL中MySQL中存储主要业务模块，例如计费模块，文章模块，信息看板模块等等，后端的框架主要使用的Spring Boot整合了Spring MVC，MyBatis，Spring Data(Mongo,QueryDSL,Redis)，使用Spring Boot 可以快速方便的对项目的配置节省开发时间。  

项目的持续集成主要使用了Jenkins对前后端项目的代码进行一键的打包部署的自动化，减少了人肉运维的痛苦。除了基本的代码工作在项目后期也担任项目的项目的运维工作，领导指示，要求把部署时间将到最短，达到让实施人员拿个U盘到某个医院在一天内就要将软硬件快速的实施完成，在我这部分工作中主要是将部署实现自动化，编写了服务所依赖的数据库和中间件的自动安装脚本（https://github.com/GuoxinL/installer ），以及Linux备份还原。  参与服务器的选型和定制。

在物联网的后端最大的问题一部分是数据收集系统的稳定性，还有一部分是对于传输协议的定义，市面上普遍的协议定义方式主要有（mqtt协议，二进制自定协议）而公司内部使用的是二进制传输协议，在二进制协议定义的上面最普遍的做法是超前的预想业务和预留字段的方式。

# 技能清单
以下均为我熟练使用的技能

- Web相关：***RESTFul标准***
- 后端框架：
  - Java: ***Spring* Cloud**, ***Spring Boot***, ***Mybatis***, _**Spring Data(Mongo,QueryDSL,Redis)**_, ***Swagger***, ***sharding-jdbc***
  - Golang: ***gin***, ***fasthttp***, ***fasthttprouter***, ***pprof***, ***log4go***, ***Gorm***, ***redigo***
- 数据库相关：***MySQL***, ***PgSQL***, ***PostGis***  缓存：***Redis***
- 运维相关：***Jenkins***, ***Jenkins pipline***, ***Docker***, ***Shell***
- 版本管理：***Svn***, ***Git***
- 云和开放平台：***阿里云***，***AWS***，***微信开发平台***

## 自我评价

- 有较好的抽象思维，面向复杂的业务抽象通用的部分，接受能力强；
- 敢于有承担责任，乐业敬业，能吃苦；
- 有团队协作精神，乐于交朋友；

# 致谢
感谢您花时间阅读我的简历，期待能有机会和您共事。

