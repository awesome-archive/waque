# 瓦雀

> 双双瓦雀行书案，点点杨花入砚池。 —— 元 叶李《暮春即事》

瓦雀可以帮你把本地的文档（markdown）目录发布到语雀上。

如果你想要...

- 返璞归真，使用 markdown；
- 选择自己喜欢的编辑器；
- 把文档维护在 GitHub 上；

瓦雀是你居家旅行，编写文档的必备工具。

> 注：文档同步是单向的，同步的文档不能再在语雀上编辑

- [瓦雀](#%E7%93%A6%E9%9B%80)
  - [安装瓦雀](#%E5%AE%89%E8%A3%85%E7%93%A6%E9%9B%80)
  - [登录语雀](#%E7%99%BB%E5%BD%95%E8%AF%AD%E9%9B%80)
  - [初始化配置](#%E5%88%9D%E5%A7%8B%E5%8C%96%E9%85%8D%E7%BD%AE)
  - [上传文档](#%E4%B8%8A%E4%BC%A0%E6%96%87%E6%A1%A3)
  - [从已有仓库导出文档](#%E4%BB%8E%E5%B7%B2%E6%9C%89%E4%BB%93%E5%BA%93%E5%AF%BC%E5%87%BA%E6%96%87%E6%A1%A3)
  - [谁在使用](#%E8%B0%81%E5%9C%A8%E4%BD%BF%E7%94%A8)

## 安装瓦雀

```bash
$ npm i -g waque
```

## 登录语雀

设置环境变量 `YUQUE_TOKEN`，语雀的 token 可以在这里获取 https://www.yuque.com/settings/tokens

## 初始化配置

在文档目录下运行下面的命令生成瓦雀的配置文件 `yuque.yml`。

这个命令会要求你输入语雀知识库的名字和要上传的文档，可以参考[配置说明](docs/configuration.md)来设置。

```bash
$ waque init
```

## 上传文档

使用下面的命令来上传文档，瓦雀会把文件名作为语雀上文档的 URL，所以文件名只能包含字母、数字、`_`和`-`（除非在文档里指定了 URL）。

```bash
$ waque upload
```

也可以指定文件上传。

```bash
$ waque upload foo.md bar.md
```

## 从已有仓库导出文档

如果你要把已有的仓库改用瓦雀管理，那么你可以用下面的命令先把文档导出成 markdown。

默认导出到当前目录下，如果指定目录，则目录要先存在。

```bash
$ waque export [DIR]
```

[导出再上传可能碰到的问题](docs/faq.md)

## 谁在使用

- [《Ant Design 实战教程》](https://www.yuque.com/ant-design/course)
