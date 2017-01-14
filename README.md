# hexo-theme-Anatole

forked from [farbox-theme-Anatole](https://github.com/hi-caicai/farbox-theme-Anatole).

This is a theme originated from a Farbox theme, which is now available in your Hexo blog. Features: two-column, responsive, clean, light, and comfortable.

![](http://labcdn.qiniudn.com/anatole/QQ%E6%88%AA%E5%9B%BE20170113193419.png)
![](http://labcdn.qiniudn.com/anatole/QQ%E6%88%AA%E5%9B%BE20170114140946.png)

### Usage

  cd blog ##folder where your Hexo blog is in
  npm install --save hexo-renderer-jade hexo-generator-archive ##these plugins are required
  git clone https://github.com/Ben02/hexo-theme-Anatole.git themes/anatole ##or you can download zip in this page

Edit your `_config.yml`, find `theme:` and change that line into `theme: anatole`, then add these lines:

  archive_generator:
    per_page: 0
    yearly: false
    monthly: false
    daily: false

### Update

  cd themes/anatole
  git pull

Attention: If you usually push your blog files to GitHub or else, you may encounter an error like:

  Changes not staged for commit:

  modified:   themes/anatole

It is supposed that you delete the `.git` folder in `themes/anatole`. In this case, you can download zip in this page to update.

### Magic

#### Customize Your Blog

You can set a certain information about your blog in `themes/anatole/_config.yml`, like `keywords`, `author`, `description`, `avatar`, and your social accounts.

#### Meta Description

If you want to set meta description information, please set `desc` property and value to each post — the better method is setting default `desc` property to your scaffolds files, just like:

  title: Lorem ipsum dolor
  date: 2015-12-31 14:49:13
  desc: Lorem ipsum dolor sit amet, consectetur.
  ---

  Lorem ipsum dolor sit amet, consectetur adipisicing elit. Totam, non numquam saepe ex ut. Deleniti culpa inventore consectetur nam saepe!

result:

  <meta name="description" content="Lorem ipsum dolor sit amet, consectetur.">

If there is no `desc` property or value, hexo-theme-Anatole will use `page.title` and `page.author` instead of it.

#### Comment Plugin

hexo-theme-Anatole supports two comment plugins: Disqus and Duoshuo. please set like this in your `theme/anatole/_config.yml`:

  disqus: seansun

Attention: To make the comment plugin work properly, please set the right username.

#### Danger Block

Use html tag with special class property to render block:

  <div class="tip">
      Something Important...
  </div>

It looks like:

![](http://labcdn.qiniudn.com/anatole/QQ%E6%88%AA%E5%9B%BE20170114141008.png)

### For A Better Experience

You can use these plugins and projects to make a better blogging experience: (They are all optional.)

1. [chenzhutian / hexo-all-minifier](https://github.com/chenzhutian/hexo-all-minifier) : lessen the size of your blog in an easy way.
2. [ihewro / Duoshuo-Disqus-theme](https://github.com/ihewro/Duoshuo-Disqus-theme) : make your Duoshuo looks like Disqus.
3. [Ben02 / 163music-APlayer-you-get-docker-mod](https://github.com/Ben02/163music-APlayer-you-get-docker-mod) : a beautiful HTML5 music player using 163 music source.

### Special Thanks to...

[pinggod/hexo-theme-apollo](https://github.com/pinggod/hexo-theme-apollo/): it inspired me so much.

### License

Anatole is released under the MIT license.

### Last but not Least

Focus on blog posts, not blog's styles. Have fun :) !
