[TOC]

Dubbo STARCHARTS:
[![Stargazers over time](https://starchart.cc/apache/incubator-dubbo.svg)](https://starchart.cc/apache/incubator-dubbo)

# Dubbo ecosystem
## 1. Dubbo framework
Dubbo is a high-performance, scalable distributed service framework, based on RPC, supporting multiple protocol invocation, service monitoring and governance.At the same time, it is a centralization framework with little invasion to application.

![](https://camo.githubusercontent.com/bcf4deea3f956beb92582b54163b743c9b0d0084/687474703a2f2f7374617469632e6f736368696e612e6e65742f75706c6f6164732f696d672f3230313131302f33303039333733375f324c68472e6a7067)

- [Offcial Website](http://dubbo.apache.org/en-us/)
- [GitHub Source](https://github.com/apache/incubator-dubbo)
- [Offcial Documents](http://dubbo.apache.org/en-us/)
- [Offcial Wiki](https://github.com/apache/incubator-dubbo/wiki)

## 2. Dubbo Presentations and Articles for Best Practice
### Dubbo principles and design
- [Service\_Framework_Practices.pdf](https://github.com/dubbo/awesome-dubbo/raw/master/slides/Service_Framework_Practices.pdf)
- [High\_Performance_Remoting.pdf](https://github.com/dubbo/awesome-dubbo/raw/master/slides/High_Performance_Remoting.pdf)
- [Framework\_Design_Principles.pdf](https://github.com/dubbo/awesome-dubbo/raw/master/slides/Framework_Design_Principles.pdf)
- [Dubbo\_RPC_Features.pdf](https://github.com/dubbo/awesome-dubbo/raw/master/slides/Dubbo_RPC_Features.pdf)
- [Dubbo\_Framework_Extensions.pdf](https://github.com/dubbo/awesome-dubbo/raw/master/slides/Dubbo_Framework_Extensions.pdf)

### Dubbo Presentations
[Dubbo open source status and future planning](
https://github.com/dubbo/awesome-dubbo/raw/master/slides/dubbo-present-and-future.pdf)

## 3. dubbo extensions and tools
### dubbox
[https://github.com/dangdangdotcom/dubbox](https://github.com/dangdangdotcom/dubbox) comes from dangdang. It mainly implements rest support based on JBoss RestEasy, upgrades dependency libraries such as spring, zk, json, and has been maintained. At present, the version of release has been 2.8.4. Documentation：
- [Developing REST style remote calls in Dubbo(RESTful Remoting)](https://dangdangdotcom.github.io/dubbox/rest.html)
- [Using efficient Java serialization in Dubbo(Kryo和FST)](https://dangdangdotcom.github.io/dubbox/serialization.html)
- [Configuring dubbox in JavaConfig mode](https://dangdangdotcom.github.io/dubbox/java-config.html)
- [Dubbo Jackson serialization use instructions](https://dangdangdotcom.github.io/dubbox/jackson.html)
- [Demo application simple operation guide](https://dangdangdotcom.github.io/dubbox/demo.html)
- [Dubbox@InfoQ](http://www.infoq.com/cn/news/2014/10/dubbox-open-source)
- [Dubbox Wiki](https://github.com/dangdangdotcom/dubbox/wiki) (edited by community volunteers)

### spring-boot-starter-dubbo
Offcial starter(maintained by mercyblitz):
- [https://github.com/apache/incubator-dubbo-spring-boot-project](https://github.com/apache/incubator-dubbo-spring-boot-project)

Avaliable starter:
- [https://github.com/cyzaoj/spring-boot-dubbo-starter](https://github.com/cyzaoj/spring-boot-dubbo-starter) can configure protocol、registry、provider<font>
- [https://github.com/linking12/spring-boot-starter-dubbo](https://github.com/linking12/spring-boot-starter-dubbo) can automatically configure and expose services.
- [https://github.com/tbud/spring-boot-starter-dubbo](https://github.com/tbud/spring-boot-starter-dubbo) added log

### dubbokeeper(dubbo-admin)
[https://github.com/dubboclub/dubbokeeper](https://github.com/dubboclub/dubbokeeper)

Dubbokeeper is an open source version of dubboadmin, a community version based on spring mvc. It also fixes some problems with the official admin and adds some necessary functions such as service statistics, dependency graph presentation, etc. At present, dubbokeeper is still in the development stage. Finally, dubbokeeper will integrate DUBBO service management system with service management and service monitoring. In particular, enhanced configuration management and service monitoring.

![](https://camo.githubusercontent.com/9719b312c10c920309bab4b17ea3189ba0562eb8/687474703a2f2f696d67302e747569636f6f6c2e636f6d2f724946565a7a362e6a706721776562)

Instructions: [http://www.cnblogs.com/yyssyh213/p/6031453.html](http://www.cnblogs.com/yyssyh213/p/6031453.html) 
Configuration of several tools: [http://www.tuicool.com/articles/u6Jzim6](http://www.tuicool.com/articles/u6Jzim6)

### dubbo monitor(bootstrap)
[http://git.oschina.net/handu/dubbo-monitor](http://git.oschina.net/handu/dubbo-monitor)

Dubbo Monitor is a monitoring system developed for Dubbo, based on improved dubbo-monitor-simple, which can be understood as an evolutionary version. The system replaces the dubbo-monitor-simple file-writing method by using a relational database (MySQL) to log. Note: it can also be changed to other Relational Database (relational database). PS: The project currently relies on version 2.8.4 of dubbox, but dubbox does not modify the monitoring code, so it can theoretically support the latest version of dubbo. The latest version from Han Du Yi She has already supported MongoDB. It is expected that it can be incorporated into dubbox as the basic skeleton of monitor.

![](
https://raw.githubusercontent.com/wiki/handuyishe/dubbo-monitor/images/screenshot.png)

### dubbo rest proxy
[https://git.oschina.net/wuyu15255872976/dubbo-rpc-proxy](https://git.oschina.net/wuyu15255872976/dubbo-rpc-proxy)

This is a magical little project that directly converts services to rest interfaces and adds parameters to URL. The interface is too rough, for fun.

### dubbo-plus
[https://git.oschina.net/bieber/dubbo-plus](https://git.oschina.net/bieber/dubbo-plus)

Provides service degradation control, enhanced cache, and other functions, which are predicted to be merged into Dubbo or dubbox.

## 4. Dubbo demos
### dubbox demos
The simplest example:
- [https://github.com/kimmking/dubbox-demos](https://github.com/kimmking/dubbox-demos)
- [webservice demo](https://github.com/dubbo/dubbo-ws-demo)

### J2EE DEMO APP
[http://git.oschina.net/vmaps/dubbo-app](http://git.oschina.net/vmaps/dubbo-app)

Dubbo-app is a J2EE distributed development infrastructure using classic technology combinations (dubbo, zookeeper, Spring, Spring MVC, MyBatis, Shiro, redis, quartz, activiti, easyui). Including core modules such as role users, authority authorization, workflow and so on. For novices, it's a good way to go from quick start to on action.

## 5. Dubbo Integration 
### dubbo + zipkin
- Distributed call chain tracing:dubbo+zipkin:dubbo+zipkin: [https://github.com/jiangmin168168/jim-framework](https://github.com/jiangmin168168/jim-framework)
- Principle:[dubbo+zipkin call chain monitoring](http://www.cnblogs.com/ASPNET2008/p/6709900.html)

### Integration of scaffolding projects for Dubbo and several common frameworks
[https://gitee.com/hackempire/emsite-parent](https://gitee.com/hackempire/emsite-parent)

### Using JMeter to do plug-in for Dubbo interface pressure test
[https://github.com/ningyu1/jmeter-plugins-dubbo](https://github.com/ningyu1/jmeter-plugins-dubbo)

## 6. Other issues
Since October 2017, it has been maintained.

v1.3


