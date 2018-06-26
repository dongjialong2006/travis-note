## Introduce

本文介绍如何用TravisCI工具发布Gitbook电子书发布到Github Pages，以便通过静态网页查看。

- Travis CI的设置
- Gitbook工具
- Github设置

### Travis CI

Travis CI 提供的是持续集成服务，它绑定 Github 上面的项目，只要有新的代码，就会自动抓取、构建和部署。

```markdown
step1: 打开(https://travis-ci.org)，用github账户登录并同步自己的repo;
step2: 打开需要构建仓库的开关；
step3: 在github仓库(需要在Travis CI上构建的项目)下添加.travis.yml文件作为Travish CI构建的配置文件；
step4: 完善.travis.yml，参考(https://docs.travis-ci.com/user/getting-started/)并提交至github对应项目下；
step5: 在Travis CI上对应项目的setting中添加必要设置，例如：GH_TOKEN；
```

### Gitbook

GitBook是使用 GitHub/Git和 Markdown(或AsciiDoc)构建漂亮书籍的命令行工具(和Node.js库)。

GitBook可以将您的内容作为网站(可定制和可扩展)或电子书(PDF，ePub或Mobi)输出。

GitBook.com 是使用 GitBook 格式创建和托管图书的在线平台。它提供托管，协作功能和易于使用的编辑器。

```markdown
step1: 安装gitbook工具集；
step2: gitbook init生成README.md和SUMMARY.md;
step3: 完善README.md和SUMMARY.md文档并提交至github上；
```

### Github

主要是配置Travis CI登录的token和访问域名。

```markdown
step1: 设置token(https://github.com/settings/tokens)并将token写入.travis.yml或配置到Travis CI对应项目的setting中；
step2: 在对应项目下创建gh-pages分支；
step3: 若用户有自己的域名，也可在项目的setting下设置，当然不设置也没问题；
```
以上用户只需更新master分支的内容即可，如无问题的话Travis CI会自动发布静态页面到gh-pages上。

### Other

本文是作者根据自己实践整理的，有不足之处，敬请谅解。