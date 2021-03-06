# ReadMe

大家好，我是助教，这里是我建立的统计计算课程的repo。请大家把作业交到这个上面来。
#### How it works

请同学们首先注册github的账号，注册后会有简单的教程。针对自己的操作系统下载git软件。

把这个repo fork到自己的账号里，方法是：点击右上角的Fork按钮。

这时你的账号里有一个repo的复制了，网站应该会自动跳转到xxx/playWithUndergraduate，其中xxx是你的账号。

我们的工作模式是，你们在自己账号中的repo里写作业，然后向我提交pull request来交作业。

首先，打开git bash，切换到你的硬盘的合适的目录(比如d盘):
```
    cd d/
```

输入

```
   git clone https://github.com/xxx/playWithUndergraduate 
```
其中xxx是你的账号。

完毕后你会发现repo已经被克隆到你的硬盘里了，进入这个repo
```
    cd playWithUndergraduate
```

然后添加一个名叫upstream的remote，保存我(助教)的repo:
```
    git remote add upstream https://github.com/kfeng123/playWithUndergraduate
```

你们在repo里添加一个自己的目录，可以以自己的学号或姓名命名：
```
    mkdir TA123456
```
然后进入这个目录：
```
    cd TA123456
```
在这份目录里新建一个文本文件，格式为markdown(.markdown或.md)。然后用markdown(语法请自行百度，5分钟以内就可以学会吧)写一份简短的自我介绍，可以只有一两行，向你的同学和我打声招呼～

以后你们写作业都放到你们自己建立的目录里，不要动其他人的目录，防止发生conflict。

现在你写好了你的个人介绍。请先更新你的repo防止冲突，然后请把repo推送到你的账号下：
```
    git add .
    git commit -m "hello world!"
    git push origin master
```
(注意第一次执行要按照提示设置你的邮箱和账号)然后在你的repo（不是我的repo！！）里已经有了你刚才写的东西了。然后请你点击New pull request向我发送pull request,按照提示填写。当我看到你的pull request并审阅你的pull request觉得没问题时，我会接受你的pull request。这样我的repo里也有了你的更改。
           
请注意两点：
1、每次你改本地repo之后，都请你push到你的github账号上，也就是说：
```
    git add .
    git commit -m "xxx"
    git push origin master
```
最好经常写。

2、请务必经常执行下面的命令，来更新你的repo（因为别的同学也会更改repo，所以你的repo并不随时都是最新的，这条命令可以让你看到别人的作业以及其他更行）。
```
    git pull --rebase upstream master
```

这就完成了作业的提交。这也是在github上为开源repo贡献代码的方式。

#### Rmarkdown

我个人建议大家使用Rmarkdown来完成作业。原因只有一个：快速。使用Rmarkdown进行写作，当你写完代码时，你会发现你自己也完成了文档的撰写。这个东西上手也是很快的。


同学们如果在软件安装、环境配置方面遇到困难，可以直接联系我邮箱，或者点击这个项目上面的那个Issues发帖(虽然那个一般是用来提价BUG的)，我会帮助大家的。^_^


~~~~~~~
