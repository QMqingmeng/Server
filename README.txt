# QM服务器群组
> Minecraft玩家社区静态站点，原生HTML/CSS/JavaScript开发，无第三方框架，支持GitHub Pages、Cloudflare Pages、Vercel静态部署。
## 📌 项目介绍
QM服务器群组是由玩家共建的Minecraft服务器集合静态网页，面向生存建筑党、红石技术宅、休闲养老类玩家。网站提供服务器介绍、社区行为规范、QQ社群入口以及网页版Minecraft游玩入口。
## 🌐 在线访问地址
- 主页面：https://qmqingmeng.github.io/Server/
- 网页版MC 1.8.8(Eaglercraft‑X)：https://qmqingmeng.github.io/Server/Minecraft/1.8.8
- 村庄农家乐子服务器页面：https://qmqingmeng.github.io/Server/farmhouse
## 📂 项目文件结构
- Server/
  - index.html：网站主页，QM服务器群组首页
  - Minecraft/
    - 1.8.8.html：网页版MC 1.8.8游戏页面
  - farmhouse/
    - index.html：村庄农家乐子服务器页面
  - README.md：项目说明文档
## ✨ 功能特性
### 🏠 主页 index.html
- 深色赛博风格UI，紫色主题配色，实现毛玻璃UI与双球体浮动光晕动画
- 完整响应式布局，PC电脑、手机移动端自动适配，使用clamp实现动态字号
- 顶部固定导航栏，下拉菜单展示全部旗下服务器
- QQ群一键复制功能，复制完成弹出成功提示，包含老旧浏览器兼容降级方案
- 社区守则毛玻璃卡片展示
- 点击页面空白区域自动关闭服务器下拉菜单
- 所有外部链接可直接修改配置
### 🎮 网页版MC 1.8.8.html
- 基于Eaglercraft‑X实现网页Minecraft 1.8.8
- 启动强制用户许可协议弹窗，同意协议后才可进入游戏
- 内置多组公益P2P联机中继节点
- 智能悬浮返回主页按钮：默认仅细边框轮廓几乎不遮挡游戏画面；点击展开显示文字并切换半透明毛玻璃；点击页面其余位置自动缩回轮廓；展开状态再次点击跳转回网站主页
- 同时支持鼠标点击与移动端touch触摸事件
## 🧰 部署方式
本项目属于纯静态网页，无需后端服务，无需数据库。
### GitHub Pages部署步骤
1. Fork该代码仓库
2. 进入仓库设置，找到Pages选项
3. 部署源选择`Deploy from a branch`，分支选择main，目录选择根目录`/ (root)`
4. 保存配置，等待1‑2分钟即可完成上线访问
> 拓展：支持在Pages设置内配置自定义域名。
## ⚙️ 自定义修改配置
### 修改全站主题颜色
打开index.html，修改CSS根变量`:root`下颜色即可全局生效：
```css
:root{
  --primary:#6C63FF;
  --accent:#FF6584;
  --bg:#0D0D2B;
  --text:#E8E8F0;
  --dim:#9999BB
}