(题目地址)[https://adworld.xctf.org.cn/task/answer?type=reverse&number=4&grade=0&id=5077&page=1](来自xctf)

题目描述：菜鸡拿到了一个被加壳的二进制文件

(题目文件)[https://github.com/KSroido/ctf-wp/blob/main/RE/simple-unpack]

# 分析思路
根据题目表述和文件名可以判断,这个文件被加壳了,于是使用著名的壳探测软件 exeinfo 进行检查:
![avatar](https://s1.ax1x.com/2020/10/30/Bt10sA.png)
