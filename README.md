eu-kirby-social-metatags
========

*Version:* 0.1a

This is a Kirby snippet (to be used with the [Kirby CMS](getkirby.com)) to be called in the page header. It's purpose is to generate FB-/OpenGraph-, TwitterCard- and Google+/Schema.org compatible meta data – the focus is the "article" content-type.

It scope somewhat differs from [@stephanbogner's](https://github.com/stephanbogner) approach in [Link Preview for Social Networks from Kirbytext](https://github.com/stephanbogner/Link-Preview-for-Social-Networks-from-Kirbytext) because it tries to mostly auto-generate everything form the site's settings.

This is an early alpha version, there's a lot to do.. If you want to help us improve it, please do so!

## Installation

### 1. Download the php file

### 2. Move it to the Kirby Snippets folder 
Move the file to the **Kirby Snippets** folder located in `Kirby ▶ site ▶ snippets`. If it does not exist, create it.

### 3. Call the snippet
Like so: ```<?php snippet('eu-kirby-social-metatags') ?>```

You'll probably want to that within your site's header snippet.

## Requirements
This thing requires a lot of fields (but most of them you'll have anyways or would want to add if you want the social metatags functionality. If any of most of the following is missing the snippet should still work, only with less meta tags output.

- ```$site->title()```
- ```$page->title()```
- ```$site->description()```→ site's meta description
- ```$page->description()```→ page's meta description
- ```$page->text()```→ page's main text content, used to generate fallback for meta description
- ```$page->featuredimage()```→ page's featured image
- ```$site->featuredimage()```→ site's featured image, used as fallback
- ```$site->twitter()```→ publishers's twitter handle
- ```$page->twitter_author()```→ authors's twitter handle
- ```$site->facebook_admin()```→ facebook admin ID

## Authors
[error:undefined design](http://error-undefined.de/)

## License

[MIT](https://opensource.org/licenses/MIT)

It is discouraged to use this plugin in any project that promotes racism, sexism, homophobia, animal abuse, violence or any other form of hate speech.