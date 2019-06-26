# 个人简历
***

## 基本信息
<table>
<tr>
<td>姓名</td>
<td>何亚东</td>
</tr>
<tr>
<td><img src='Image/call.png' width='20' height="20"/></td>
<td>15800010611</td>
</tr>
<tr>
<td><img src='Image/email.png'  width='20' height="20"/></td>
<td>nuxseme@gmail.com</td>
</tr>
<tr><td><img src='Image/sunyatsen.jpg'  width='20' height="20"/></td>
<td>中山大学软件工程</td></tr>
<tr><td><img src='https://nuxseme.github.io/resume/Image/GitHub.ico'  width='20' height="20"/></td>
<td><a href="http://github.com/nuxseme" target="_blank" style="text-decoration:none;" >github</a></td></tr>
</tr>
<tr><td><img src='https://nuxseme.github.io/resume/Image/home.ico'  width='20' height="20"/></td>
<td><a href="http://nuxseme.com" target="_blank" style="text-decoration:none;">个人主页</a></td></tr>
</table>


## 工作经历
### 小满科技

- 职位：php高级开发工程师
- 任职时间：2017.5--今
- 主要任务：CRM核心模块开发和维护

#### 邮件
- 项目描述
CRM管理系统主要管理用户的客户，邮件，单据，产品等数据。邮件作为用户的商业沟通的主要载体，需要搜索，分发，多个终端同步等各种业务操作。

##### 邮件消费队列

- 主要任务
大量的邮件收下来之后需要，对每封邮件回调处理，由于处理的业务比较多，耗时比较长。
- 解决方案
队列
- 实现
php+swoole

遇到的问题: 静态变量不断增长导致内存oom

##### 邮件模块重构

- 主要任务
对旧的邮件逻辑重新整理
- 解决方案和实现
1 抽象成代理类处理，逻辑分离
2 数据表根据稀疏度拆分成横表和竖表
3 统一回调逻辑，接受接口调用和队列消费
 
##### 邮件多端同步

- 主要任务
桌面端，app端，web端邮件同步
- 解决方案
http+pb
- 实现
1 数据变更操作埋点，记录下version
2 终端存储邮件的同步下来的最新的version
3 心跳机制比较终端和同步服务器的版本号的差异
4 终端将差异数据拉取到本地，同时更新终端的最新版本号

#### AI推荐

- 主要任务
根据用户所处行业和喜好，给用户推荐潜在的客户。推荐算法在其他组，主要负责业务侧，数据展示，模板选择，性能等任务
- 解决方案
服务多次请求+服务降级处理确保服务可用
- 实现
1 数据和接口预处理
2 降级策略
3 缓存降低接口压力

#### 通用统计查询

- 主要任务
模拟数据库查询，解决数据库异构，用户自定义查询的需求
- 解决方案
1 查询配置
2 数据处理配置
3 格式化配置
4 查询优化器
5 模型配置

- 实现
定义基础数据模型，数据适配器，数据通用查询逻辑


### 通淘国际有限公司  

- 职位：系统开发工程师
- 任职时间：2016.6--2017.5
- 主要任务：tomtop供应链项目协作开发，图片系统独立开发，其他部门子系统功能对接

#### Tomtop供应链项目
- 项目描述  
供应链是跨境电商平台子项目，负责将国外的各地的各大平台的热门的sku销售到国内  

- 主要任务  
php中间件开发，将单一的js+java结构解耦。由js负责业务逻辑，java负责后台接口转向php负责数据展示，java负责服务提供。java设计之初用来提供细粒度的api接口，js负责业务组装，大量的业务逻辑暴露到前端，散落到各处。
- 解决方案  
增加php中间层，由php负责数据渲染，数据缓存，数据同步，用户认证等功能
- 实现  
1 mongodb+crontab实现数据同步  
2 redis实现数据缓存  
3 项目基础ddd+Yii2


#### 图片管理系统

- 项目描述  
统一处理各个项目需要用到图片存储，url映射，图片缩略，压缩，比较等功能 

- 主要任务  
公司各个项目拥有自己的图片管理系统（erp、webpos、M站），维护和调度十分繁琐。了解各个系统的业务，将图片处理的功能整合，同时提供各个系统需要的api服务

- 实现  
1 项目框架Yii2  
2 缩略策略gd、gm  
3 Yii2 路由映射，动态请求缓存  

- 不足  
1 框架可采用轻框架  
2 权限，操作日志，系统日志需要完善  
3 图片响应时间需要优化  
   

---
### 野大豆科技 （2015.4-2016.5）

- 职位：系统开发工程师
- 任职时间：2015.4--2016.5
- 主要任务：负责业务分析，需求处理，各个项目的开发维护，测试环境的维护

#### 微分销平台
- 项目描述  
基于微信平台的o2o系统
- 主要任务  
独立负责会员模块，商品模块的开发，负责订单流程维护和调优
- 实现  
1 框架基础php+swoole  
2 mongodb日志数据存储  
3 mongodb+mysql数据存储  
4 memcache缓存  
5 用swoole实现定时器，插件	  

#### 微支付
- 项目描述  
第三方支付平台
- 主要任务  
流程分析,消息队列,ab数据压测
- 实现  
1 ab 数据压测   
2 mongo日志记录  
3 redis+swoole实现消息队列  

#### 微抢购  
#### 拼团


## 开源项目和作品

### 开源项目
 
#### [iphp](http://github.com/nuxseme/iphp)    
> php+swoole搭建的简易框架，包含自动加载，路由解析，http解析，错误处理，环境检测等功能。定时器，插件等功能待完善
#### [nuxseme](http://www.nuxseme.com)
> github+hexo+Next+travis-ci搭建的博客项目  
> 修改了Next主题部分代码  
> 采用travis-ci自动测试部署 

## 技术文章

- [sso流程解析](http://nuxseme.com/sso/sso)
- [nginx+lua+graphicsmagick实时生成缩略图](http://nuxseme.com/php/nginx+lua+graphicsmagick%E5%AE%9E%E6%97%B6%E7%94%9F%E6%88%90%E7%BC%A9%E7%95%A5%E5%9B%BE) 
- [ssh原理和流程](http://nuxseme.com/ssh/ssh%E5%8E%9F%E7%90%86%E5%92%8C%E6%B5%81%E7%A8%8B)
- [more...](http://nuxseme.com)

## 技能清单

- Web开发：PHP
- Web框架：ThinkPHP/Yii2/CXSV
- web服务器：apache，nginx
- 前端框架：Bootstrap/VUE.js
- 数据库相关：MySQL/PgSQL/PDO/SQLite/MonogoDB
- 持续集成：Phing/travis-ci
- 版本管理、文档和自动化部署工具：Svn/Git/Composer/Xdebug
- 单元测试：PHPUnit
- 开放平台：微信应用开发
- 云服务器:腾讯云，centos
- 脚本语言：shell
- 自动监控：notify

未来计划：   
- php源码   
- 面向对象    
- 设计模式  
- nodoJS  
- ddd  
- java  
- docker  
- 持续集成，自动部署  
- 测试  
- 网络编程



## 致谢
感谢您花时间阅读我的简历

