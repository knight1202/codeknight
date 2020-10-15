---
title: Hello World
---
Welcome to [Hexo](https://hexo.io/)! This is your very first post. Check [documentation](https://hexo.io/docs/) for more info. If you get any problems when using Hexo, you can find the answer in [troubleshooting](https://hexo.io/docs/troubleshooting.html) or you can ask me on [GitHub](https://github.com/hexojs/hexo/issues).

## Quick Start

### Create a new post

``` bash
$ hexo new "My New Post"
```

More info: [Writing](https://hexo.io/docs/writing.html)

### Run server

``` bash
$ hexo server
```

More info: [Server](https://hexo.io/docs/server.html)

### Generate static files

``` bash
$ hexo generate
```

More info: [Generating](https://hexo.io/docs/generating.html)

### Deploy to remote sites

``` bash
$ hexo deploy
```

``` java
 public RetVal info(@PathVariable String token){
        MemberCenterVo memberCenterVo = new MemberCenterVo();
        Claims claims = JwtUtils.checkJWT(token);
        String nickname = (String) claims.get("nickname");
        String avatar = (String) claims.get("avatar");
        String id = (String) claims.get("id");
        memberCenterVo.setId(id);
        memberCenterVo.setAvatar(avatar);
        memberCenterVo.setNickname(nickname);
        return RetVal.success().data("memberCenterVo",memberCenterVo);
    }

```
More info: [Deployment](https://hexo.io/docs/one-command-deployment.html)
