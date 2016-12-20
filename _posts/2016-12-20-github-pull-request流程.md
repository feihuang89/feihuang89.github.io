---
layout: post
title: github pull request流程
date: 2016年12月20日下午7:05
---
#### github pull request流程
1.fork别人在github上面的远程仓库，相当于拷贝，不影响原仓库

2.cd 本地存放fork仓库的文件夹,执行git clone 'fork的仓库地址'，地址使用https方式

3.此处如果需要使用ssh方式,需要本地生成ssh key,终端输入命令:ssh-keygen -t rsa -C 'github的邮箱'

4.输入保存路径以及文件名：默认/Users/Africa/.ssh/id_rsa

![输入ssh key保存路径](/Users/Africa/Desktop/屏幕快照 2016-12-20 下午6.15.15.png)

5.输入密码并确认密码之后的成功状态:

![ssh key生成成功](/Users/Africa/Desktop/屏幕快照 2016-12-20 下午6.26.40.png)

6.打开github->点击头像->Settings->SSH and GPC keys->New SSH key，打开刚才生成的GitHub.pub公钥，复制公钥到github;

7.执行git clone 'ssh地址'

8.修改代码后,到原代码仓库发起pull request

9.原仓库作者review之后，同意会执行merge操作