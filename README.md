# README

## 安裝的流程 使用終端機

``` bash

# 安裝 Hexo CLI
npm install -g hexo-cli

# 建立專案
hexo init gitpag
cd gitpag
npm install

# 安裝 Fluid 主題
cd themes
git clone https://github.com/fluid-dev/hexo-theme-fluid.git fluid
cd ../
cp themes/fluid/_config.yml _config.fluid.yml

# 修改 _config.yml
theme: fluid

# 確認主題是否成功
hexo clean && hexo g
hexo s

# GitHub Pages 自動部署
npm install hexo-deployer-git --save

# 修改 _config.yml
deploy:
  type: git
  repo: https://github.com/username/username.github.io.git
  branch: main

or

deploy:
  type: git
  repo: https://github.com/username/hexo-blog.git
  branch: gh-pages

# 部署
hexo clean && hexo g
hexo deploy


#建立三個頁面 
hexo new page archives
hexo new page categories
hexo new page tags


tags
self
分享
傳訊
接訊


categories
自我成長

```
