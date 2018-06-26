# Gitbook操作

安装好Gitbook命令后，在创建好的Github电子书项目下(master分支，当然用户也可以自建分支，最终在合并
到master分支)，执行如下命令：
- gitbook init           // 初始化README.md和SUMMARY.md
- edit README.md         // 电子书的介绍文档
- edit SUMMARY.md        // 电子书的目录结构
- gitbook init           // 根据目录结构定义的内容生成各章节的目录、README.md和***.md文件
- edit every README.md   // 完善各章节的介绍
- edit every ***.md      // 完善各章节的内容
- edit .travis.yml       // 编写Travis CI的配置文件
将以上编译完成的文档，提交至Github即可。

注：
`Markdown`的语法结构请自行学习。
`.travis.yml`文档的语法请参考[语法帮助](https://docs.travis-ci.com/)。
