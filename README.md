# hexo-theme-Anatole

forked from [farbox-theme-Anatole](https://github.com/hi-caicai/farbox-theme-Anatole).

Anatole is a theme originated from a Farbox theme, now available in your Hexo blog. Features: two-column, responsive, clean, light, and comfortable.

![](http://labcdn.qiniudn.com/anatole/QQ%E6%88%AA%E5%9B%BE20170113193419.png)
![](http://labcdn.qiniudn.com/anatole/QQ%E6%88%AA%E5%9B%BE20170114145625.png)

[中文文档](https://munen.cc/tech/Anatole.html) | [English Wiki](#usage)

## Usage

```bash
cd blog ##folder where your Hexo blog is in
npm install --save hexo-renderer-jade hexo-generator-archive ##these plugins are required
git clone https://github.com/Ben02/hexo-theme-Anatole.git themes/anatole ##or you can download zip in this page
```

Edit your `_config.yml`, find `theme:` and change that line into `theme: anatole`, then add these lines:

```yaml
archive_generator:
  per_page: 0
  yearly: false
  monthly: false
  daily: false
```

## Update

```bash
cd themes/anatole
git pull
 ```

Attention: If you usually push your blog files to GitHub or else, you may encounter an error like:

```bash
Changes not staged for commit:

modified:   themes/anatole
```

It is supposed that you delete the `.git` folder in `themes/anatole`. In this case, you can download zip in this page to update.

## Magic

### Customize Your Blog

You can set a certain information about your blog in `themes/anatole/_config.yml`, like `keywords`, `author`, `description`, `avatar`, and your social accounts.

### English Display

Just delete `/themes/anatole/languages/zh-cn.yml`.

### Meta Description

If you want to set meta description information, please set `desc` property and value to each post — the better method is setting default `desc` property to your scaffolds files, just like:

```yaml
title: Lorem ipsum dolor
date: 2015-12-31 14:49:13
desc: Lorem ipsum dolor sit amet, consectetur.
---

  Lorem ipsum dolor sit amet, consectetur adipisicing elit. Totam, non numquam saepe ex ut. Deleniti culpa inventore consectetur nam saepe!
```

result:

```html
<meta name="description" content="Lorem ipsum dolor sit amet, consectetur.">
```

If there is no `desc` property or value, hexo-theme-Anatole will use the first 150 characters of your post instead of it.

### Index Description

hexo-theme-Anatole truncates text of your posts after 160 characters in index, category, and tag pages. To change the length, you can edit `/layout/mixins.jade`, find `p!= truncate(strip_html(summary), {length: 160})` then change the number `160`.

To control each description of your posts, please set `summary` property and value to each post — the better method is setting default `summary` property to your scaffolds files, like [that](#meta-description). (Thank [@tanwenhai](https://github.com/tanwenhai))

### Comment Plugin

hexo-theme-Anatole supports two comment plugins: Disqus and Duoshuo. please set like this in your `theme/anatole/_config.yml`:

```yaml
disqus: seansun
```

Attention: To make the comment plugin work properly, please set the right username.

### Danger Block

Use html tag with special class property to render block:

```html
<div class="tip">
  Something Important...
</div>
```

It looks like:

![](http://labcdn.qiniudn.com/anatole/QQ%E6%88%AA%E5%9B%BE20170114141008.png)

### Customize Your Navbar

Hexo-theme-Anatole shows links of 'About' and 'Links' pages in navbar by default. You should create two pages whose permalinks are `about` and `links`. If you would like to change those two urls or delete them, you can edit `/layout/partrial/nav.jade`.  

## For A Better Experience

You can use these plugins and projects to make a better blogging experience: (They are all optional.)

1. [chenzhutian / hexo-all-minifier](https://github.com/chenzhutian/hexo-all-minifier) : lessen the size of your blog in an easy way.
2. [ihewro / Duoshuo-Disqus-theme](https://github.com/ihewro/Duoshuo-Disqus-theme) : make your Duoshuo looks like Disqus.
3. [Ben02 / 163music-APlayer-you-get-docker-mod](https://github.com/Ben02/163music-APlayer-you-get-docker-mod) : a beautiful HTML5 music player using 163 music source.

## Special Thanks to...

[pinggod/hexo-theme-apollo](https://github.com/pinggod/hexo-theme-apollo/): it inspired me so much.

## License

Anatole is released under the MIT license.

## Last but not Least

Focus on blog posts, not blog's styles. Have fun :) !
