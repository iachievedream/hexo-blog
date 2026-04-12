# README

## 安裝的流程 使用終端機

``` bash

# 安裝 Hexo CLI
npm install -g hexo-cli

# 建立專案 [以資料夾為 gitpag 為例 可更換名稱]
hexo init gitpag
cd gitpag

git init
git add .
git commit -m "init"
npm install

# 安裝 Fluid 主題
==========
AI：幫我安裝 https://github.com/fluid-dev/hexo-theme-fluid 在 package 管理工具中
下方為操作回應：
==========
npm install --save hexo-theme-fluid 2>&1
cp node_modules/hexo-theme-fluid/_config.yml _config.fluid.yml

## 修改 _config.yml
theme: landscape
改為
theme: fluid

## 確認主題是否成功 [如果設定沒吃到 需要重起 須先將原先的 hexo s 關閉]
hexo clean && hexo g && hexo s


# GitHub Pages 自動部署
npm install hexo-deployer-git --save

## 修改 _config.yml
deploy:
  type: git
  repo: https://github.com/username/hexo-blog.git
  branch: gh-pages


# 建立三個頁面
hexo new page archives
hexo new page categories
hexo new page tags


# 部署
hexo clean && hexo g && hexo deploy


[Utterances GitHub App](https://github.com/apps/utterances)
文章需添加下列 才會無法顯示留言板
comments: false


# hexo 以及 SEO 的關係
以及如何優化
優化後會有那些的好處

npm install hexo-generator-sitemap
npm install hexo-generator-baidu-sitemap

```
