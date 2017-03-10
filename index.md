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

### 通淘国际有限公司  

- 职位：系统开发工程师
- 任职时间：2016.6--今
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

