# hexo-theme-mint
一个清爽的双栏hexo博客主题, Another simple and elegant theme for Hexo.
<img src="https://pic1.zhimg.com/v2-d5b1a201ec0aced140a5a56f67fef4f0_b.png" width="100%"/>
<p align="center">
    <a href="https://github.com/yuttian/hexo-theme-mint" target="_blank">
        <img src="http://yuttian.github.io/img/responsive.png">
    </a>
</p>
&emsp;&emsp;Theme **mint** relies on [Hexo-Theme-spfk][1], thanks for the author [luuman][2]. Fix some bugs, change lots of styles, add several features. And then I made the theme. mint is mainly designed for clean . I change styles and add functions, meanwhile, try hard to keep this theme simple, stupid and clear. Theme DEMO: [reno's Blog][3]

[1]: https://github.com/luuman/hexo-theme-spfk
[2]: https://github.com/luuman
[3]: https://yuttian.github.io/

### Installation

```
git clone https://github.com/yuttian/hexo-theme-mint.git themes/mint
```

Change theme field in Hexo root's _config.yml file. 

```
theme: mint
```

### Update

```
cd themes/mint
git pull
```

### Configuration

#### Internationalization
Use internationalization to present your site in different languages.

https://hexo.io/docs/internationalization.html

```yaml
# Hexo Configuration
## Docs: http://hexo.io/docs/configuration.html

# Site
language: en
```

##### Available Languages

| Code           | -                     | -        | 
|----------------|:-----------------------:|:----------:|
| **en**         | English               | 英语     | 
| **zh-Hans**    | Chinese (Simplified)  | 大陆简体 |  
| **zh-Hant-HK** | Chinese (Traditional) | 港澳繁體 | 
| **zh-Hant-TW** | Chinese (Traditional) | 台灣正體 |

> **Any Contribution is Welcome！**

#### 0. Post Excerpt
There are two ways to show excerpt in homepage. 

- a: <!-- more -->

``` diff
title: Hello World
date: 2015-12-03 00:00:00
---
<Excerpt in index> 
+ <!-- more -->
<The rest of contents文>
```
- b: description in Front-matter

``` diff
title: Hello World
date: 2015-12-03 00:00:00
+ description: "Welcome to Hexo! This is your very first post."
---
<Contents>
```

> Description only support plain text

> Set the value of description with quotes to avoid unexpected error `:`



#### 1. About Page:
cd to your hexo folder and run this code:


```
hexo new page about
```

#### 2. Tags Cloud Page:

```
hexo new page tags
```

> Post with several categories

#### 3. Background image:

Find or change background images in folder: 

> `/mint/source/background/`

Setting in `themes/mint/_config.yml`:

`
background_image: 5
`

- Default value is 5, free to modify the number

- "5": show 5 images form bg-1.jpg to bg-5.jpg in `/mint/source/background/`

- "0": remove background image and use white-gray theme

> [Saving JPEGs for the Web: Setting Photoshop Up for Progressive JPEGs](http://peteschuster.com/2013/01/saving-jpegs-for-the-web-setting-photoshop-up-for-progressive-jpegs/)

> Optimize images with PhotoShop (JPEG, Quality 0, Progressive)

#### 4. Highlight Style:
Set inline_code to style highlight text & Chose a highlight theme for code block.

```
highlight_style:
  #on: true
  inline_code: 1
  code_block: 1
```

Set `on: true` to enable this feature

highlight theme from https://github.com/chriskempson/tomorrow-theme

#### 5. Comment:
Disqus, duoshuo and youyan is supported, enable ONE of them in theme's "_config.yml".

#### 6. 404 Page:

```
hexo new page 404
```
And then set `permalink: /404` in `/mint/404/index.md` front matter.

#### 7. RSS Feed:

Install plugin: [hexo-generator-feed](https://github.com/hexojs/hexo-generator-feed)

#### 8. Sitemap for SEO:

Install plugin: [hexo-generator-seo-friendly-sitemap](https://github.com/ludoviclefevre/hexo-generator-seo-friendly-sitemap)

Baidu: [hexo-generator-baidu-sitemap](https://github.com/coneycode/hexo-generator-baidu-sitemap)

#### 9. Apple Touch icon:

The Path is `/mint/source/apple-touch-icon.png`

[Recommended size: 180*180](https://realfavicongenerator.net/blog/apple-touch-icon-the-good-the-bad-the-ugly/)
