使用方法：

## 初始
1. 打开终端 Terminal
2. 输入 `cd Document/syt-blog`

## 新建文件

在终端输入`./new.sh "文件名"` 即可创建文件 + 图片存放文件夹

例如 `./new.sh "abc"` 会在 `/source/_posts`文件夹下创建一个名为 `2021-03-21-abc.md` 的文件（用于写作），同时还会在 `/source/_pics`文件夹下创建一个 `2021-03-21-abc` 的文件夹用来存放这篇文章涉及的图片。

注意：文件名不能用空格，建议用英文，如有多个单词，用短横线连接。

打开该文章，会有

```
<img src='/pics/2021-03-21-abc/xx.png' style='zoom:100%, margin: 0 auto; display: block;'>"
```

如果有文章图片，只需要修改上面语句中 `xx.png`将其改成图片名称即可。 zoom是缩放比例，可以根据图片适当调整。

## 预览文章内容

在终端输入 `hexo s`，在浏览器窗口中输入 `http://localhost:4000/` 即可查看预览版本。

按 Ctrl + C 这两个键退出预览内容。

## 发布文章

当预览完成没有问题后，可以将文章推送到 github 上，具体方法如下：

1. 在终端输入

`git add .` 这句是新增改动
`git commit -m "update: upload articles"` 这句是注释；
`git push` 这句是将文字内容推送到 github 上。

这就完成了所有工作。
