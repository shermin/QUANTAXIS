# QUANTAXIS 量化金融策略框架

[![Github workers](https://img.shields.io/github/watchers/yutiansut/quantaxis.svg?style=social&label=Watchers&)](https://github.com/yutiansut/quantaxis/watchers)
[![GitHub stars](https://img.shields.io/github/stars/yutiansut/quantaxis.svg?style=social&label=Star&)](https://github.com/yutiansut/quantaxis/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/yutiansut/quantaxis.svg?style=social&label=Fork&)](https://github.com/yutiansut/quantaxis/fork)

![version](https://img.shields.io/badge/Version-%200.4.0/beta-orange.svg)
![build](https://travis-ci.org/yutiansut/QUANTAXIS.svg?branch=0.4.0-alpha)
[![StackShare](https://img.shields.io/badge/tech-stack-0690fa.svg?style=flat)](https://stackshare.io/yutiansut/quantaxis)
![QAS](https://img.shields.io/badge/QAS-%200.0.8-brown.svg)
![Pypi](https://img.shields.io/badge/Pypi-%200.4.0-blue.svg)
![python](https://img.shields.io/badge/python-%203.6/win/ubuntu-darkgrey.svg)
![Npm](https://img.shields.io/badge/Npm-%200.4.0-yellow.svg)
![author](https://img.shields.io/badge/Powered%20by-%20%20yutiansut-red.svg)
![license](https://img.shields.io/badge/License-%20MIT-brightgreen.svg)


```shell
 ...................................................................................................................... 
 ..########.....##........##..........##.........####........##...##########.......##......##......###...##.....######.. 
 .##......## ...##........##.........####........##.##.......##.......##..........###.......##....##.....##...##.....##. 
 ##........##...##........##........##.##........##..##......##.......##.........####........#...##......##...##......## 
 ##........##...##........##.......##...##.......##...##.....##.......##.........##.##.......##.##.......##....##....... 
 ##........##...##........##......##.....##......##....##....##.......##........##..###.......###........##.....##...... 
 ##........##...##........##......##......##.....##.....##...##.......##.......##....##.......###........##......###.... 
 ##........##...##........##.....##........##....##......##..##.......##......##......##.....##.##.......##........##... 
 ##........##...##........##....#############....##.......##.##.......##.....###########.....##..##......##.........##.. 
 ###.......##...##........##...##...........##...##.......##.##.......##....##.........##...##...##......##...##.....##. 
 .##......###....##......###..##.............##..##........####.......##...##..........##..###....##.....##....##.....## 
 ..#########......########...##..............###.##..........##.......##..##............##.##......##....##.....##....## 
 ........#####.....................................................................................................####.. 
 ...................................................................................................................... 
 ..........................Copyright..yutiansut..2017......QUANTITATIVE FINANCIAL FRAMEWORK.............................. 
 ...................................................................................................................... 
 ........................................................................................................................ 
```
QUANTAXIS量化金融策略框架,是一个面向中小型策略团队的量化分析解决方案. 我们通过高度解耦的模块化以及标准化协议,可以快速的实现面向场景的定制化解决方案.QUANTAXIS是一个渐进式的开放式框架,你可以根据自己的需要,引入自己的数据,分析方案,可视化过程等,也可以通过RESTful接口,快速实现多人局域网/广域网内的协作.

QUANTAXIS与国内很多优秀的量化平台的区别在于,QA更多关注的是用户体验和实际情景,对于用户需求会有较多的优化.所以会更加注重开放性,引入自定义的便捷性,以及团队协作的细节处理.好比如自定义的数据引入,自定义的策略图表对比,自定义的风险和策略组合管理等等.

> 欢迎加群讨论: [群链接](https://jq.qq.com/?_wv=1027&k=4CEKGzn) 

> 更新内容详见: https://github.com/yutiansut/QUANTAXIS/blob/0.4.0-beta/update_log.md

> 如有问题,可以在github上发[issue](https://github.com/yutiansut/QUANTAXIS/issues), 也可以QQ 279336410,QQ群 563280067联系我

> 关键词: 纯本地框架/局域网协作/高度自定义/渐进式框架




![QUANTAXIS LOGO](http://i1.piimg.com/1949/62c510db7915837a.png)

<!-- TOC -->

- [QUANTAXIS 量化金融策略框架](#quantaxis-量化金融策略框架)
    - [说明文档 (Updating)](#说明文档-updating)
    - [QUANTAXIS-Stardand-Protocol](#quantaxis-stardand-protocol)
    - [部署问题:](#部署问题)
    - [回测Webkit插件概览](#回测webkit插件概览)
    - [适用场景](#适用场景)

<!-- /TOC -->

## 说明文档 (Updating)
[地址](https://yutiansut.gitbooks.io/quantaxis/)
![](http://i1.piimg.com/567571/dc3c811a5afcb4fb.png)
![新的回测框架](http://osnhakmay.bkt.clouddn.com/quantaxis_new_backtest_engine.png)
## QUANTAXIS-Stardand-Protocol
QUANTAXIS 标准化协议和未来协议

QUANTAXIS-Stardand-Protocol 版本号0.0.8

详情参见  [QUANATXISProtocol](https://github.com/yutiansut/QUANTAXIS/tree/0.3.8-dev-RC-ARP/QUANTAXISProtocol)

## 部署问题:

- Windows/Linux(ubuntu) 已测试通过
- python3.6(开发环境) python2 回测框架不兼容(attention! 之后会逐步用更多高级语法)   [*] 如果需要交易,请下载32位的python3.6
- nodejs 需要安装>7的版本,来支持es6语法
- mongodb是必须要装的


一个简易demo(需要先安装并启动mongodb,python版本需要大于3)
```shell

#install python3.6 in linux
sudo add-apt-repository ppa:jonathonf/python-3.6
sudo apt-get update
sudo apt-get install python3.6
wget https://bootstrap.pypa.io/get-pip.py
sudo -H python3.6 get-pip.py
#



git clone https://github.com/yutiansut/quantaxis
cd quantaxis 
(sudo) pip install -e . # 一定要用这种方法,python setup.py install方法无法解压 安装在本目录下的开发模式
在命令行输入 quantaxis 进去quantaxis CLI
quantaxis> save

随意新建一个目录:

在命令行输入 quantaxis 进去quantaxis CLI


输入examples 在目录下生成一个示例策略


python  backtest.py

```
![简易策略](http://i1.buimg.com/1949/44f692d0c9d6fed2.png)

启动网络插件(nodejs 版本号需要大于6,最好是7)
```shell
cd QUANTAXISWebkit
(sudo) npm run install

(sudo) npm install forever -g
cd backend
(sudo) forever start bin/www
cd ..
cd web
(sudo) npm run dev
```
会自动启动localhost:8080网页端口,用账户名admin,密码admin登录

## 回测Webkit插件概览

![](http://i2.muimg.com/567571/736ba4adda9fac85.png)
![](http://i2.muimg.com/588926/345e924a45cae6e5.png)
![](http://i1.piimg.com/1949/7b6e2fc347220f7b.png)
![](http://i1.piimg.com/567571/09bd05c3698f2d38.png)
![](http://i1.piimg.com/567571/053ac3e3850f8f60.png)

## 适用场景
![适用场景](http://i2.buimg.com/567571/e2e7b31b1f9a4307.png)



