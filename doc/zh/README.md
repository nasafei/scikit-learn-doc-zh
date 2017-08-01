# scikit-learn 文档

本节包含http://scikit-learn.org中显示的完整手册和网页。
要生成完整的网页，包括示例图库（这可能需要一段时间）：

    make html

或者，如果你不想建立示例图库：

    make html-noplot

这应该创建目录 _build/html 中的所有文档

要构建PDF手册，请运行

    make latexpdf


该网站托管在github，可以手动更新（针对版本）
通过推送到 https://github.com/scikit-learn/scikit-learn.github.io 存储库。

在上传网站之前，建议您运行OptiPNG。
Matplotlib生成的PNG文件往往大于20％，而且它们是耗费我们带宽。 您可以运行OptiPNG ::

    make optipng

# 开发文档自动化构建

名为“docbuilder”的Rackspace云服务器正在不断地构建主分支，以更新网站的 http://scikit-learn.org/dev 树。

此服务器的配置管理在：

    https://github.com/scikit-learn/sklearn-docbuilder

