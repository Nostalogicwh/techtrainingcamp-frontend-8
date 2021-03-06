# 2048Online

# From：techtrainingcamp-frontend-8 

2048是一款经典的益智类游戏，欢迎来到我们构建的2048世界！

## 技术栈：

Vue + Node.js + Socket.io

## 在线游戏地址

[点此进入2048online游戏](http://47.110.94.236)

## 部分游戏页面

![image](https://github.com/H-jialing/techtrainingcamp-frontend-8/blob/main/src/assets/img/pic1.png)
![image](https://github.com/H-jialing/techtrainingcamp-frontend-8/blob/main/src/assets/img/pic2.png)
![image](https://github.com/H-jialing/techtrainingcamp-frontend-8/blob/main/src/assets/img/pic3.png)
![image](https://github.com/H-jialing/techtrainingcamp-frontend-8/blob/main/src/assets/img/pic4.png)

## 本地环境配置

1、git clone代码并解压

2、cd到目录文件夹并npm install

3、在AgainstGame.vue中，将socket地址切换为localhost（如果不切换将连接后台服务器）

const socket = io.connect('http://127.0.0.1:8081')

//const socket = io.connect('http://47.110.94.236')


(localhost的后台集成在webpack的webpack.dev.conf.js文件中，监听8081端口）

4、npm run dev启动项目，后端自动启动

5、在浏览器输入localhost：8080进入项目

## 单人游戏模式

模式介绍：

（1）经典模式：2 + 2 = 4， 4 + 4 = 8...合成2048即可获胜！小心不要无路可走哦。

（2）限时模式：在经典模式的背景下加入了计时器，争分夺秒的合成方块吧！

（3）速度模式：更加紧张刺激的模式，别犹豫！再不活动棋盘就要立刻Game Over了哦~

（在单人模式中还有彩蛋哦，你发现了吗？）

## 多人PK模式

在多人模式中，每一个房间只能容纳两位玩家，房间与房间之间的通信是分开的。在多人PK模式中，你可以自由设定游戏难度（简单/中等/困难）以及游戏时间（X分钟），并等待你的对手加入房间。当两人都在房间时房主可以开始游戏，在PK中你可以看到自己和对手的实时分数，并在游戏结束时根据分数结算胜负关系。我们还开发了聊天功能，里面还有表情包可以用哦，在游戏的过程中也别忘了和小伙伴愉快交流~

(1) 简单：有5%的概率生成32新格子，帮助你更快速的合成2048
(2) 正常：经典的2048游戏模式
(3) 困难：每次新生成两个格子

## Beta版本

我们其实还有很多很多的Idea在路上,比如更好的游戏对战互动，更好的用户交互体验，以及更少的bug(T_T)。但由于时间有限，我们在第一版上线的正式版中不能完全呈现出来。我们还会继续维护这个线上的游戏，希望更多的玩家可以 Join And Have Fun！


