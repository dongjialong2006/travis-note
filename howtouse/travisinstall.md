# Travis安装

安装 Ruby版的包travis工具，该工具作者仅用来加密token，其命令如下：
```markdown
travis encrypt REPO_TOKEN=<TOKEN>
```
将生成的token，添加至Travis CI对应项目的setting下(如`GH_TOKEN`)，同时将该环境变量设置到`.travis.yml`中，如下：
```markdown
github_token:
    secure: $GH_TOKEN
```

当然，用户也可以不安装该工具包，直接将Github上生成的token添加至Travis CI也可以。