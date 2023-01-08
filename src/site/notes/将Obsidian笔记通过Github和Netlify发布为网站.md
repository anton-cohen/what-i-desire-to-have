---
{"dg-publish":true,"permalink":"/obsidian-github-netlify/","tags":"gardenEntry"}
---


# 将Obsidian笔记通过Github和Netlify发布为网站
1. 在Obsidian中安装Digital Garden插件：设置→第三方插件（→关闭安全模式）→浏览→搜索到Digital Garden→安装→启用；
2. 在GitHub中打开仓库：https://github.com/oleeskild/digitalgarden→点击绿色的Deploy to Netlify→Connect to GitHub→Authorize netlify→键入Repository name→Save & Deploy→该网站会生成形如https://clinquant-peony-d53fb0.netlify.app的网址；
3. 打开网址：https://github.com/settings/tokens/new?scopes=repo→在Note处键入名称（如Obsidian-Netlify）→在Expiration中勾选No expiration→Generate token→复制该token；
4. 打开Obsidian→设置→第三方插件→Digital Garden→输入GitHub repo name、GitHub Username及GitHub token，并关闭；
5. 在Obsidian创建一个新的笔记，并在开头输入如下内容：
    ```
    ---
    dg-publish: true
    dg-home: true
    ---
    ```
    其中dg-publish设置该笔记是否需要被发布到互联网上，dg-home设置该笔记是否作为网站首页；
6. 点击Obsidian左侧边栏的小树苗图标→在Unpublished中点击Publish unpublished notes按钮，即可发布相应笔记；
7. 打开Netlify中生成的形如https://clinquant-peony-d53fb0.netlify.app的网址，即可浏览笔记。