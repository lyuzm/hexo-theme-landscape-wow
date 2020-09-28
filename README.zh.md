# Landscape-Wow

 一个基于[Landscape](http://hexo.io/hexo-theme-landscape/)主题修改的魔兽世界风格的 [Hexo] 主题。

- [示例](https://lyuzm.gitee.io)

## 安装说明

### 安装

``` bash
$ git clone https://github.com/lyuzm/hexo-theme-landscape-wow.git themes/landscape-wow

**Landscape-wow 需要 Hexo 2.4 及以上版本.** 如果你想启用 RSS，还需要 [hexo-generate-feed] 插件。

### 开启

修改 `_config.yml`中的 `theme` 设置为 `landscape-wow`.

### 更新

``` bash
cd themes/landscape-wow
git pull
```

## 配置

``` yml
# Header
menu:
  Home: /
  Archives: /archives
rss: /atom.xml

# Content
excerpt_link: Read More
fancybox: true

# Sidebar
sidebar: right
widgets:
- category
- tag
- tagcloud
- archives
- recent_posts

# Miscellaneous
google_analytics:
favicon: /favicon.png
twitter:
google_plus:
```

- **menu** - 导航菜单
- **rss** - RSS链接
- **excerpt_link** - "阅读更多"链接在摘录文章的底部。`false`隐藏该链接。
- **fancybox** - 开启 [Fancybox]
- **sidebar** - 侧栏样式。你可以选择 `left`, `right`, `bottom` 或者 `false`.
- **widgets** - 侧栏中显示的小工具
- **google_analytics** - Google Analytics ID
- **favicon** - Favicon path
- **twitter** - Twiiter ID
- **google_plus** - Google+ ID

## 特点

### Fancybox

Landscape 使用 [Fancybox] 来展示你的图片.你可以使用Markdown语法或fancybox标签插件来添加你的图片。

```
![img caption](img url)

{% fancybox img_url [img_thumbnail] [img_caption] %}
```

### 侧边栏

您可以通过编辑 `sidebar`设置将您的侧边栏放在网站的左侧、右侧或底部。

Landscape 提供了5个内置小部件:

- category
- tag
- tagcloud
- archives
- recent_posts

所有这些都是默认启用的，您可以在`widget`设置中编辑它们。


[Hexo]: https://hexo.io/
[Fancybox]: http://fancyapps.com/fancybox/
[Font Awesome]: http://fontawesome.io/
[Grunt]: http://gruntjs.com/
[hexo-generate-feed]: https://github.com/hexojs/hexo-generator-feed
