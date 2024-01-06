
# README
```如何搭建自己的Blog```

## 搭建和部署

```关于我的Blog```

> **Hexo(Theme:Butterfly) + Deploy(GithubPage)**

## 前置基础

```个人认为最重要的```

1.会看文档，会看文档，会看文档

2.感兴趣，身体各个内脏情况良好

3.熟练运用搜索引擎

## 参考文章

```关于主题参考官方文档即可```

[Hexo官方文档](https://hexo.io/zh-cn/docs/)

---

# 重置系统后有感

```因为某些驱动问题重置了系统，再一次安装Hexo出现了新的问题，再结合之前的问题，我打算重新完善一下我的README```

## 参考文章（第三方）
```让我们看看其它人是怎么搭建的（详细）```


1.真的是全网最详细的版本了，稍微注意就是node的下载地址的打开：
https://blog.csdn.net/cat_bayi/article/details/128725230

2.这篇文章建议和上一篇对照着看：
https://blog.csdn.net/sinat_37781304/article/details/82729029

3.这篇是一个朋友在自己blog上写的，可以参考他的ssh-keys绑定：
https://imgod.me/posts/39317.html#%E9%80%9A%E8%BF%87-ssh-keys-%E7%BB%91%E5%AE%9A-GitHub

4.Butterfly除了有[官方文档](https://butterfly.js.org/)还有[官方文档的衍生改版](https://butterfly.zhheo.com/)，可塑性很强，其它主题应该也有自己的衍生版本

## 我踩过的坑

### 配置文件

blog根目录下的配置文件(_config.yml)和主题下面的配置文件是不一样的，配文件的时候不要配错了，除了我之外我也见到其他人有配错文件的情况。

建议一劳永逸，在blog的根目录下再创建一个配置文件(eg._config.butterfly.yml 和blog的配置文件区分开来)，然后把主题的配置文件粘贴到我们刚刚新创建的配置文件（具体情况参考官方文档，安装文档（一）的末尾处）

### 重装node

下载文件选择的后缀名为.msi
下错了打开原的安装包进行remove或repair
没事尽量不要选择更新版本（）

### 部署 github page

最开始我按照文档(Hexo一键部署)配的：

> repo: git@github.com:MercuryRandom/mercuryrandom.github.io

第一天还可以正常使用，结果第二天再次部署就出了问题：
应该得再后面再加上个```git```
> repo: git@github.com:MercuryRandom/mercuryrandom.github.io.git

如果是从仓库中直接将对应路径贴过去再最后也是有(.git)的 (?)

### 路径
```Painful Forever```

关于 node/Git 路径参考 ：```参考文档(第三方)1.``` ，如果出现node和npm显示正常而hexo出问题的情况可以试着把系统路径的node和node_global分别都加上（不断排查）



关于 git-bash ：第一次下载的时候因为没把 git-bash 顺便装在powershell 上，导致后面出现了很多不必要的麻烦
https://blog.csdn.net/ggh_567/article/details/135262857

### 图片

注意格式

### 关于README部署
看这篇博文
https://blog.csdn.net/qq_36759224/article/details/91981824

### 如果找不到问题？
```不是问题的问题```

反复配路径发现没问题，反复重装还是失败，那很可能是```ssh-keys```的锅，把密钥重新配一遍，相信一切都会好起来的！


