
Starter theme for [Hexo](http://www.hexo.io) implemented with [Jade](http://jade-lang.com/) and [Less](http://lesscss.org/). This theme is intended be a starting point for anyone who is interested in creating Hexo theme using Jade.

This theme includes [Hashgrid](http://www.hashgrid.com) for development helper. Just press 'g' on your local instance to see it in action.

To set up your own dev helper follow these instructions:

- For CSS, just put your stylesheets inside `[theme_root]/css/_dev/` and import them in `[theme_root]/css/dev.less`.
- For Javascripts, since there is no bundling available, you have to include any third party library manually. See the last line of `[theme_root]/layout/_partial/site/head.jade`, include your third party scripts before `!= js("javascript/dev")` and initialize those scripts on `[theme_root]/source/javascript/dev.js`.

### Why Jade?

- Less typing because Jade uses indentation to convey html tag structure
- More flexible template inheritance with extend and block

### Why Less?

Stylus is great, but it does not fully support CSS syntax. Thus if you already have some base stylesheets in CSS you have to convert them to Stylus first to be safe. By using Less, you can just drop in your CSS files and it will work.

## Installation

Get to your Hexo directory and install the dependencies first.

```bash
npm install hexo-renderer-jade --save
npm install hexo-renderer-less --save
```

Clone this repository to your Hexo themes folder and set your `theme` in `_config.yml` to `jade-starter`.

```bash
git clone git://github.com/widatama/hexo-jade-starter.git themes/jade-starter
```
