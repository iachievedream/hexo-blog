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
hexo clean
hexo g
hexo s
```
