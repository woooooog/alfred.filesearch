# alfred.filesearch
alfred workflow, 文件(夹)名和文件内容的快速检索

## 介绍

基于 [fd](https://github.com/sharkdp/fd), [ag](https://github.com/ggreer/the_silver_searcher), [hanz2piny](https://github.com/brain-zhang/hanz2piny/tree/branches/pipein)

三种模式: 
1. 慢加载快检索 + 拼音检索 + 缓存 文件名. 默认触发词 en
2. 较快检索 文件(夹)名, 可以全路径或包不包含文件夹搜索. 默认触发词 f
3. 检索文件夹下所有包含文本的文件内容, 多关键词并集检索, 可指定文件类型. 默认触发词 t

⌘+⏎ : 在文件夹中显示
⌘+L : 显示备注文本
⏎ : 打开文件
shift/⌘+Y : 预览文件

## 效果

环境: macos 10.15.6 intel i9处理器 macbookpro

80万文件检索名称速度2.93秒:

![f-80](images/f-80.jpg)

1.28万文件检索名称速度0.04秒:

![f-1.28](images/f-1.28.jpg)

1.28万文件, 总400MB+文本 的文件内容检索速度0.34秒:

![t-1.28-400M](images/t-1.28-400M.jpg)

拼音检索:

![en](images/en.jpg)


## 安装
1. 下载 alfredworkflow 文件: https://github.com/aitsc/alfred.filesearch/releases
2. 双击 File.Search.alfredworkflow
3. 进入alfred workflow设置, 双击对应 Script Filter 模块, 可以在其中看到检索路径等参数修改的提示, 修改路径保存后用于自己的路径进行检索. 还可以复制 Script Filter 及后面操作, 然后修改触发关键词和检索路径. ~表示用户文件夹.

