# **自用termux资源**
---

## ***一. clash使用***

```
// 1.安装clash服务
   pkg install clash

// 2.下载clash订阅配置 clash.yaml可以修改名称也可以加文件夹，后缀不变就行
   curl -o clash.yaml http://192.168.*************

// 3.启动clash服务 前台或后台
   clash -f clash.yaml                       //前台运行，可以看输出日志
   nohup clash -f clash.yaml >> clash.out &  //后台运行，日志输出到clash.out
```
---

## ***二. package-subconverter***

termux编译的subconverter，用作clash订阅链接规则转换

*[subconverter使用方法](https://github.com/tindy2013/subconverter)*

pref.ini为配置文件，用的是acl4ssr的online规则，也可以自己参考使用方法编辑，编辑好之后执行命令：
```
./subconverter                                //前台运行，可以看输出日志
nohup ./subconverter >> subconverter.out &    //后台运行，日志输出到subconverter.out
```

然后根据使用方法获取你的订阅链接，使用软件或者termux的clash订阅代理

