(题目地址)[https://adworld.xctf.org.cn/task/answer?type=reverse&number=4&grade=0&id=5077&page=1](来自xctf)

题目描述：菜鸡拿到了一个被加壳的二进制文件

(题目文件)[https://github.com/KSroido/ctf-wp/blob/main/RE/simple-unpack]

# 分析思路
根据题目表述和文件名可以判断,这个文件被加壳了,于是使用著名的壳探测软件 exeinfo 进行检查:
![avatar](https://s1.ax1x.com/2020/10/30/Bt10sA.png)

```
detect UPX
```

作为知名开源壳,upx脱壳还是很简单的

前往(upx官网)[ http://upx.github.io ],下载upx脱壳组件

下载完成后将upx.exe的绝对路径(即,D:/.../.../upx.exe,C:/.../.../upx.exe  诸如此类)添加至环境变量(目的是可以在任意目录下使用cmd中的upx命令)
![](https://s1.ax1x.com/2020/10/30/Btr9Rs.png)
在cmd中输入
```
upx -d (要脱壳文件的绝对路径)
```
[![BtruW9.md.png](https://s1.ax1x.com/2020/10/30/BtruW9.md.png)](https://imgchr.com/i/BtruW9)
