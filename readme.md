# nbb3210.github.io
## github+hexo搭建geocafe主页

### 域名问题

- 先有一个域名**www.geocafe.cn**


- 阿里云域名解析
  - `CHAME` `*` `默认` `nbb3210.github.io.`
- github域名设置
  - `Settings` `GitHub Pages` `Custom domain` `www.geocafe.cn`
  - 或者生成文件**CHAME**，添加`www.geocafe.cn`

### 开发模式

- 在文件夹**cafe** 下`hexo init cafe`，生成骨架
- 在项目**nbb3210.github.io**下新建分支**develop**，将**cafe**文件夹下的内容拷贝至此，可将**cafe**文件夹删除
- 安装`yarn add hexo-depolyer-git`，并[配置](https://hexo.io/zh-cn/docs/deployment.html)
- 通过`hexo g`生成内容，再通过`hexo d`将内容推送至**master**主分支，从而实现开发
- `hexo g`之前在文件**_config.yml**，中修改**message**