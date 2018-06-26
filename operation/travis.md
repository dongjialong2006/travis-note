# Travis CI操作

构建并发布Github上的Gitbook项目，操作流程如下：
- 打开https://travis-ci.org
- 用Github账号登录Travis CI并同步项目信息
- 打开要构建和发布的项目开关
- 进入该项目的setting，设置环境变量，如：GH_TOKEN等
- start builder

如果异常，构建会报错，根据提示查找错误即可。