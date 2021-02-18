---
title: Github Pages + Hexo 建立博客站点
date: 2021-02-18 10:02:26
tags: #Blog #Github #Web #Geek #Hexo #Setup
---

# 环境

- Windows 10 Pro 1909
- NodeJS
- Hexo
- Git
- Github Pages

# 参考

[通过Git将Hexo博客部署到服务器 - 简书](https://www.jianshu.com/p/e03e363713f9)

[Hexo配合github搭建网站 - 简书](https://www.jianshu.com/p/3e6083a2b498)

[手把手教你用Hexo+Github 搭建属于自己的博客_gdutxiaoxu的博客（微信公众号 stormjun94）-CSDN博客](https://blog.csdn.net/gdutxiaoxu/article/details/53576018)

[[Hexo + GitHub Pages] 零成本的 HTTPS 建站大法 - 神代綺凜の随波逐流](https://moe.best/tutorial/hexo-github-pages.html)

# 踩坑

- **仅当** Github Repository 命名为 `<accountname>.github.com` 时，Github Pages 默认域名是 `<accountname>.github.io`，即**个人或公司页面**；否则为`<accountname>.github.com/<repository name>`，即**项目页面**。后者会导致 Hexo 的默认 url 出错。

- 如果站点部署在子目录（subdirectory）下，需在 Hexo 配置文件`_config.yml` 中配置为：

	```yml
	url: http://example.com/child
	```

- Hexo 初始化：

	```bash
	hexo init
	```
需要空目录