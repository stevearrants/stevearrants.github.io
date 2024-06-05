# Beautiful Jekyll

[![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg)](https://www.paypal.me/daattali/20)
[![Gem Version](https://badge.fury.io/rb/beautiful-jekyll-theme.svg)](https://badge.fury.io/rb/beautiful-jekyll-theme)

> *Copyright 2018 [Dean Attali](https://deanattali.com)*

**Beautiful Jekyll** is a ready-to-use template to help you create an awesome website quickly. Perfect for personal sites, blogs, or simple project websites.  [Check out a demo](https://deanattali.com/beautiful-jekyll) of what you'll get after just two minutes.  You can also look at [my personal website](https://deanattali.com) to see it in use, or see examples of websites other people created using this theme [here](#showcased-users-success-stories).

**If you enjoy this theme, please consider [supporting me](https://www.paypal.me/daattali/20) for developing and maintaining this template.**

<p align="center">
  <a href="https://www.paypal.me/daattali">
    <img src="https://www.paypalobjects.com/en_US/i/btn/btn_donate_LG.gif" />
  </a>
</p>

### Table of contents

- [Prerequisites](#prerequisites)
- [Build your website in 3 steps](#build-your-website-in-3-steps)
- [Add your own content](#add-your-own-content)
- [Last important thing: YAML front matter ("parameters" for a page)](#last-important-thing-yaml-front-matter-parameters-for-a-page)
- [Features](#features)
- [Creating a User Page vs a Project Page](#creating-a-user-page-vs-a-project-page)
- [Showcased users (success stories!)](#showcased-users-success-stories)
- [Advanced: local development](#advanced-local-development-using-docker)
- [FAQ and support](#faq-and-support)
- [Credits and contributions](#credits)

## Prerequisites

- You need to have a GitHub account. If you don't have one, [sign up here](https://github.com/join) - it takes one minute. This is where your website will live - if you sign up with username `johnsmith` then your website will be `https://johnsmith.github.io`.
- It would be helpful to understand what Markdown is and how to write it. Markdown is just a way to take a piece of text and format it to look a little nicer.  For example, this whole instruction set that you're reading is written in markdown - it's just text with some words being bold/larger/italicized/etc. I recommend taking 5 minutes to learn markdown [with this amazingly easy yet useful tutorial](https://markdowntutorial.com/).

- **SIMPLE**: The primary goal of Beautiful Jekyll is to allow literally *anyone* to create a website in a few minutes.
- **Modern**: Uses the latest best practices and technologies to achieve nearly perfect scores on Google Chrome's Audit.
- **Mobile-first**: Designed to look great on both large-screen and small-screen (mobile) devices.
- **Highly customizable**: Many personalization settings such as changing the background colour/image, adding a logo.
- **Flexible usage**: Use Beautiful Jekyll directly on GitHub or via a Ruby gem - choose the best [development method](#build-your-website-in-3-steps) for you.
- **Battle-tested**: By using Beautiful Jekyll, you'll be joining 50,000+ users enjoying this theme since 2015.
- **SEO and social media support**: Customize how your site looks on Google and when shared on social media.
- **Comments support**: Add comments to any page using either [Disqus](https://disqus.com/), [Facebook comments](https://developers.facebook.com/docs/plugins/comments), [Utterances](https://utteranc.es/), [Staticman](https://staticman.net), or [giscus](https://giscus.app).
- **Tags**: Any blog post can be tagged with keywords, and an index page is automatically generated.
- **Analytics**: Easily integrate Google Analytics, or other analytics platforms, to track visits to your website.
- **Search**: Let users easily find any page using a Search button in the navigation bar.
- **Photos support**: Any page can have a full-width cover photo and thumbnail.
- **RSS**: An RSS feed is automatically created, so you can even host a podcast easily with Beautiful Jekyll.

<h2 id="sponsors">Sponsors 🏆</h2>

Developing and maintaining Beautiful Jekyll takes a lot of time and effort - thank you to anyone who helps fund this effort!

- [LoadView-Testing](https://www.loadview-testing.com/products/jmeter-load-testing/)
- [DoFollow](https://dofollow.co.uk/)
- [\_hyp3ri0n](https://hyperiongray.com)

**[Become a sponsor for Beautiful Jekyll and unlock special rewards\!](https://github.com/sponsors/daattali/sponsorships?tier_id=39856)**

# Build your website in 3 steps

There's a very easy way to use this theme, and there's a hard way. For most people (including myself!), the easy route is recommended. If you're an advanced user and want to tinker with the hard way (using ruby gems), then [skip the easy way](https://github.com/daattali/beautiful-jekyll#the-hard-way-using-ruby-gems) if you know what you're doing.

## The easy way (recommended!)

Getting started is *literally* as easy as 1-2-3 :smile:
Scroll down to see the steps involved, but here is a 40-second video just as a reference as you work through the steps.

![Installation steps](img/install-steps.gif)

### 1. Fork this repository

(Assuming you are on this page and logged into GitHub) Fork this repository by clicking the *Fork* button on the top right corner. Forking means that you now copied this whole project and all the files into your account.

### 2. Rename the repository to `<yourusername>.github.io`

This will create a GitHub User page ready with the **Beautiful Jekyll** template that will be available at `https://<yourusername>.github.io` within a couple minutes.  To do this, click on *Settings* at the top (the cog icon) and there you'll have an option to rename.

### 3. Customize your website settings

Edit the `_config.yml` file to change all the settings to reflect your site. To edit the file, click on it and then click on the pencil icon (watch the video tutorial above if you're confused).  The settings in the file are fairly self-explanatory and I added comments inside the file to help you further. Any line that begins with a pound sign (`#`) is a comment, and the rest of the lines are actual settings.

Another way to edit the config file (or any other file) is to use [prose.io](https://prose.io/), which is just a simple interface to allow you to more intuitively edit files or add new files to your project.

After you save your changes to the config file (by clicking on *Commit changes* as the video tutorial shows), your website should be ready in a minute or two at `https://<yourusername>.github.io`. Every time you make a change to any file, your website will get rebuilt and should be updated in about a minute or so.

You can now visit your shiny new website, which will be seeded with several sample blog posts and a couple other pages. Your website is at `https://<yourusername>.github.io` (replace `<yourusername>` with your user name). Do not add `www` to the URL - it will not work!

**Note:** The video above goes through the setup for a user with username `daattalitest`. I only edited one setting in the `_config.yml` file in the video, but **you should actually go through the rest of the settings as well. Don't be lazy, go through all the settings :)**

## Add your own content

To add pages to your site, you can either write a markdown file (`.md`) or you can write an HTML file directly.  It is much easier to write markdown than HTML, so I suggest you do that (use the [tutorial I mentioned above](https://markdowntutorial.com/) if you need to learn markdown). You can look at some files on this site to get an idea of how to write markdown. To look at existing files, click on any file that ends in `.md`, for example [`aboutme.md`](./aboutme.md). On the next page you can see some nicely formatted text (there is a word in bold, a link, bullet points), and if you click on the pencil icon to edit the file, you will see the markdown that generated the pretty text. Very easy!

In contrast, look at [`index.html`](./index.html). That's how your write HTML - not as pretty. So stick with markdown if you don't know HTML.

Any file that you add inside the [`_posts`](./_posts) directory will be treated as a blog entry.  You can look at the existing files there to get an idea of how to write blog posts.  After you successfully add your own post, you can delete the existing files inside [`_posts`](./_posts) to remove the sample posts, as those are just demo posts to help you learn.

As mentioned previously, you can use [prose.io](https://prose.io/) to add or edit files instead of doing it directly on GitHub, it can be a little easier that way.

## Last important thing: YAML front matter ("parameters" for a page)

In order to have your new pages use this template and not just be plain pages, you need to add [YAML front matter](https://jekyllrb.com/docs/front-matter/) to the top of each page. This is where you'll give each page some parameters that I made available, such as a title and subtitle. I'll go into more detail about what parameters are available later. If you don't want to use any parameters on your new page (this also means having no title), then use the empty YAML front matter:

```
---
---
```

If you want to use any parameters, write them between the two lines. For example, you can have this at the top of a page:

```
---
title: Contact me
subtitle: Here you'll find all the ways to get in touch with me
---
```

You can look at the top of [`aboutme.md`](./aboutme.md) or [`index.html`](./index.html) as more examples.

**Important takeaway: ALWAYS add the YAML front matter, which is two lines with three dashes, to EVERY page. If you have any parameters, they go between the two lines.**    
If you don't include YAML then your file will not use the template.

## Features

### Mobile-first
**Beautiful Jekyll** is designed to look great on both large-screen and small-screen (mobile) devices. Load up your site on your phone or your gigantic iMac, and the site will work well on both, though it will look slightly different.

### Customizable

Many personalization settings in `_config.yml`, such as setting your name and site's description, changing the background colour/image, setting your avatar to add a little image in the navigation bar, customizing the links in the menus, customizing what social media links to show in the footer, etc.

### Allowing users to leave comments

If you want to enable comments on your site, Beautiful Jekyll supports either the [Disqus](https://disqus.com/) comments plugin, [Facebook](https://developers.facebook.com/docs/plugins/comments) comments, [Staticman](https://staticman.net) or [just-comments](https://just-comments.com). If any of these are set in the configuration file, then all blog posts will have comments turned on by default. To turn off comments on a particular blog post, add `comments: false` to the YAML front matter. If you want to add comments on the bottom of a non-blog page, add `comments: true` to the YAML front matter.

#### Disqus comments

To use Disqus, simply sign up to [Disqus](https://disqus.com/) and add your Disqus shortname to the `disqus` parameter in the `_config.yml` file.

#### Facebook comments

To use Facebook comments, create a Facebook app using [Facebook developers](https://developers.facebook.com/docs/apps/register), and add the Facebook App ID to the `fb_comment_id` parameter in `_config.yml`.

#### Staticman comments

To use Staticman, you first need to invite `staticmanlab` as a collaborator to your repository (by going to your repository **Settings** page, navigate to the **Collaborators** tab, and add the username `staticmanlab`), and then accept the invitation by going to `https://staticman3.herokuapp.com/v3/connect/github/<username>/<repo-name>`. Lastly, fill in your `repository` and `branch` in the Staticman section of `_config.yml`.

#### Just-Comments comments

To use Just-comments you first need to have an account. After you just need to copy the API key to the just-comments property in `_config.yml` file.

### Adding Google Analytics to track page views

Beautiful Jekyll lets you easily add Google Analytics to all your pages. This will let you track all sorts of information about visits to your website, such as how many times each page is viewed and where (geographically) your users come from.  To add Google Analytics, simply sign up to [Google Analytics](https://www.google.com/analytics/) to obtain your Google Tracking ID, and add this tracking ID to the `google_analytics` parameter in `_config.yml`.

### Sharing blog posts on social media

By default, all blog posts will have buttons at the bottom of the post to allow people to share the current page on Twitter/Facebook/LinkedIn.  You can choose to enable/disable specific social media websites in the `_config.yml` file. You can also turn off the social media buttons on specific blog posts using `social-share: false` in the YAML front matter.

### RSS feed

Beautiful Jekyll automatically generates a simple RSS feed of your blog posts, to allow others to subscribe to your posts.  If you want to add a link to your RSS feed in the footer of every page, find the `rss: false` line in `_config.yml` and change it to `rss: true`.

### Page types

- **post** - To write a blog post, add a markdown or HTML file in the `_posts` folder. As long as you give it YAML front matter (the two lines of three dashes), it will automatically be rendered like a blog post. Look at the existing blog post files to see examples of how to use YAML parameters in blog posts.
- **page** - Any page outside the `_posts` folder that uses YAML front matter will have a very similar style to blog posts.
- **minimal** - If you want to create a page with minimal styling (ie. without the bulky navigation bar and footer), assign `layout: minimal` to the YAML front matter.
- If you want to completely bypass the template engine and just write your own HTML page, simply omit the YAML front matter. Only do this if you know how to write HTML!

### YAML front matter parameters

These are the main parameters you can place inside a page's YAML front matter that **Beautiful Jekyll** supports.

Parameter   | Description
----------- | -----------
title       | Page or blog post title
subtitle    | Short description of page or blog post that goes under the title
tags        | List of tags to categorize the post. Separate the tags with commas and place them inside square brackets. Example: `[personal, analysis, finance]`
cover-img   | Include a large full-width image at the top of the page. You can either provide the path to a single image (eg. `"/path/to/img"`) , or a list of images to cycle through (eg. `["/path/img1", "/path/img2"]`). If you want to add a caption to an image, then you must use the list notation (use `[]` even if you have only one image), and each image should be provided as `"/path/to/img" : "Caption of image"`.
thumbnail-img | For blog posts, if you want to add a thumbnail that will show up in the feed, use `thumbnail-img: /path/to/image`. If no thumbnail is provided, then `cover-img` will be used as the thumbnail. You can use `thumbnail-img: ""` to disable a thumbnail.
comments    | If you want do add comments to a specific page, use `comments: true`. Comments only work if you enable one of the comments providers (Facebook, disqus, staticman, utterances, giscus) in `_config.yml` file. Comments are automatically enabled on blog posts but not on other pages; to turn comments off for a specific post, use `comments: false`.

## Parameters for SEO and social media sharing

These parameters let you control what information shows up when a page is shown in a search engine (such as Google) or gets shared on social media (such as Twitter/Facebook).

Parameter   | Description
----------- | -----------
share-title | A title for the page. If not provided, then `title` will be used, and if that's missing then the site title (from `_config.yml`) is used.
share-description | A brief description of the page. If not provided, then `subtitle` will be used, and if that's missing then an excerpt from the page content is used.
share-img   | The image to show. If not provided, then `cover-img` or `thumbnail-img` will be used if one of them is provided.

## Less commonly used parameters

These are parameters that you may not use often, but can come in handy sometimes.

Parameter   | Description
----------- | -----------
readtime    | If you want a post to show how many minutes it will take to read it, use `readtime: true`.
show-avatar | If you have an avatar configured in the `_config.yml` but you want to turn it off on a specific page, use `show-avatar: false`.
social-share | By default, every blog post has buttons to share the page on social media. If you want to turn this feature off, use `social-share: false`.
nav-short   | By default, the navigation bar gets shorter after scrolling down the page. If you want the navigation bar to always be short on a certain page, use `nav-short: true`
gh-repo   | If you want to show GitHub buttons at the top of a post, this sets the GitHub repo name (eg. `daattali/beautiful-jekyll`). You must also use the `gh-badge` parameter to specify what buttons to show.
gh-badge  | Select which GitHub buttons to display. Available options are: [star, watch, fork, follow]. You must also use the `gh-repo` parameter to specify the GitHub repo.
last-updated | If you want to show that a blog post was updated after it was originally released, you can specify an "Updated on" date.
layout      | What type of page this is (default is `post` for blog posts and `page` for other pages). See _Page types_ section below for more information.

## Advanced parameters

These are advanced parameters that are only useful for people who need very fine control over their website.

Parameter   | Description
----------- | -----------
footer-extra | If you want to include extra content below the social media icons in the footer, create an HTML file in the `_includes/` folder (for example `_includes/myinfo.html`) and set `footer-extra` to the name of the file (for example `footer-extra: myinfo.html`). Accepts a single file or a list of files.
before-content | Similar to `footer-extra`, but used for including HTML before the main content of the page (below the title).
after-content | Similar to `footer-extra`, but used for including HTML after the main content of the page (above the footer).
head-extra   | Similar to `footer-extra`, but used if you have any HTML code that needs to be included in the `<head>` tag of the page.
language    | HTML language code to be set on the page's &lt;html&gt; element.
full-width  | By default, page content is constrained to a standard width. Use `full-width: true` to allow the content to span the entire width of the window.
js          | List of local JavaScript files to include in the page (eg. `/assets/js/mypage.js`)
ext-js      | List of external JavaScript files to include in the page (eg. `//cdnjs.cloudflare.com/ajax/libs/underscore.js/1.8.2/underscore-min.js`). External JavaScript files that support [Subresource Integrity (SRI)](https://developer.mozilla.org/en-US/docs/Web/Security/Subresource_Integrity) can be specified using the `href` and `sri` parameters eg.<br/>`href: "//code.jquery.com/jquery-3.1.1.min.js"`<br/>`sri: "sha256-hVVnYaiADRTO2PzUGmuLJr8BLUSjGIZsDYGmIJLv2b8="`
css         | List of local CSS files to include in the page
ext-css      | List of external CSS files to include in the page. External CSS files using SRI (see `ext-js` parameter) are also supported.
googlefonts | List of Google fonts to include in the page (eg. `["Monoton", "Lobster"]`)
gh-repo   | If you want to show GitHub buttons at the top of a post, this sets the GitHub repo name (eg. `daattali/beautiful-jekyll`). You must also use the `gh-badge` parameter to specify what buttons to show.
gh-badge  | Select which GitHub buttons to display, available options are: [star, watch, fork, follow]. You must also use the `gh-repo` parameter to specify the GitHub repo.

### Advanced features (including how to use a custom URL address for your site)

I wrote [a blog post](https://deanattali.com/2015/03/12/beautiful-jekyll-how-to-build-a-site-in-minutes/) describing some more advanced features that I used in my website that are applicable to any Jekyll site.  It describes how I used a custom URL for my site (deanattali.com instead of daattali.github.io), how to add a Google-powered search into your site, and provides a few more details about having an RSS feed.

## Creating a User Page vs a Project Page

If you're not sure what the difference is, you can probably safely ignore this section.

If you want to use this theme to host a website that will be available at `https://YOURUSERNAME.github.io`, then you do not need to read this section. That is called a User Page, you can only have one User Page in your GitHub account, and it is what you get by default when forking this project.

If you want to use this theme to create a website for a particular repository, it will be available at `https://YOURUSERNAME.github.io/REPONAME`, and that is called a [Project Page](https://help.github.com/articles/user-organization-and-project-pages/). You can have a Project Page for each repository you have on GitHub. There are two important things to note when creating a project page:

1. In the configuration file (`_config.yml`), you should set `baseurl` to be `/projectname` instead of `""`.
2. Project Pages are served from a branch named `gh-pages`, and you should be generating all the website content on that branch. When you fork Beautiful Jekyll, you'll already have a `gh-pages` branch but you should delete it and generate it again from the `master` branch. The reason is that the `gh-pages` branch in its current form does not have the updated code of Beautiful Jekyll, so you need to create that branch from the `master` branch (which is where all my new features and work go into).

## Showcased users (success stories!)

To my huge surprise, Beautiful Jekyll has been used in over 500 websites in its first 6 months alone! Here is a hand-picked selection of some websites that use Beautiful Jekyll.

Want your website featured here? [Contact me](https://deanattali.com/aboutme#contact) to let me know about your website.

### Project/company websites

| Website | Description |
| :------ |:----------- |
| [repidemicsconsortium.org/](https://www.repidemicsconsortium.org/) | R Epidemics Consortium |
| [vaccineimpact.org](https://www.vaccineimpact.org/) | Vaccine Impact Modelling Consortium |
| [derekogle.com/fishR](http://derekogle.com/fishR/) | Using R for Fisheries Analyses |
| [bigdata.juju.solutions](http://bigdata.juju.solutions) | Creating Big Data solutions Juju Solutions |
| [joecks.github.io/clipboard-actions](http://joecks.github.io/clipboard-actions/) | Clipboard Actions - an Android app |
| [deanattali.com/shinyjs](http://deanattali.com/shinyjs/) | shinyjs - an R package |
| [blabel.github.io](http://blabel.github.io) | Library for canonicalising blank node labels in RDF graphs |
| [reactionic.github.io](http://reactionic.github.io) | Create iOS and Android apps with React and Ionic |
| [ja2-stracciatella.github.io](http://ja2-stracciatella.github.io) | Jagged Alliance 2 Stracciatella |
| [ddocent.com](http://ddocent.com/) | RADSeq Bioinformatics and Beyond |
| [guitarlessons.org](https://www.guitarlessons.org/) | Free online guitar lessons for all |
| [terremotocentroitalia.info](https://www.terremotocentroitalia.info/) | Information about the 2016 Italy earthquake |


### Personal websites

| Website | Who | What |
| :------ |:--- | :--- |
| [deanattali.com](https://deanattali.com) | Dean Attali | Creator of Beautiful Jekyll |
| [ouzor.github.io](http://ouzor.github.io) | Juuso Parkkinen | Data scientist |
| [derekogle.com](http://derekogle.com/) | Derek Ogle | Professor of Mathematical Sciences and Natural Resources |
| [melyanna.github.io](http://melyanna.github.io/) | Melyanna | Shows off her nice art |
| [chauff.github.io](http://chauff.github.io/) | Claudia Hauff | Professor at Delft University of Technology |
| [kootenpv.github.io](http://kootenpv.github.io/) | Pascal van Kooten | Data analytics |
| [sjackman.ca](http://sjackman.ca) | Shaun Jackman | PhD candidate in bioinformatics |
| [anudit.in](http://www.anudit.in/) | Anudit Verma | Engineering student |
| [sharepointoscar.github.io](http://sharepointoscar.github.io) | Oscar Medina | Independent Hacker |
| [ocram85.com](https://ocram85.com) | Marco Blessing | A personal blog about PowerShell and automation |
| [khanna.cc](https://khanna.cc/) | Harry Khanna | Law and software |

## Advanced: Local development using Docker

Beautiful Jekyll is meant to be so simple to use that you can do it all within the browser. However, if you'd like to develop locally on your own machine, that's possible too if you're comfortable with command line. Follow these simple steps set that up with Docker:

1. Make sure you have [Docker](https://www.docker.com/) installed.

2. Clone your repository locally.

    ```bash
    git clone https://github.com/<your_username>/<your_username>.github.io.git
    ```

3. Run the following shell commands to build the docker image and start the container for the first time:

    ```bash
    cd <repository_folder>
    docker build -t beautiful-jekyll "$PWD"
    docker run -d -p 4000:4000 --name beautiful-jekyll -v "$PWD":/srv/jekyll beautiful-jekyll
    ```

Note: If you encounter write permission problems with `Gemfile.lock`, try:

```bash
touch Gemfile.lock
chmod a+w Gemfile.lock
```

Now that Docker is set up, you do not need to run the above steps again. You can now view your website at http://localhost:4000/. You can start the container again in the future with:

```bash
docker start beautiful-jekyll
```

And you can stop the server with:

```bash
docker stop beautiful-jekyll
```

Whenever you make any changes to `_config.yml`, you must stop and re-start the server for the new config settings to take effect.

Disclaimer: I personally am NOT using local development so I don't know much about running Jekyll locally. If you follow this route, please don't ask me questions because unfortunately I honestly won't be able to help!

## FAQ and support

If you need any help, I suggest heading over to the [Jekyll support forum](https://talk.jekyllrb.com/).

Beautiful Jekyll is actively used by thousands of people with wildly varying degrees of competency, so it's impossible to answer all the questions that may arise. Below are answers to a few very common questions. Most questions that I get asked are not directly related to this theme, and instead are more general questions about Jekyll or web development. Many such questions can be answered by reading the [Jekyll documentation](https://jekyllrb.com/) or with Google.

#### How do I change the number of posts per page OR the colour of the navigation bar OR the image in the navigation bar OR ...?

Beautiful Jekyll is built to be very customizable, and as such, many questions about "how do I change ..." can be answered by looking at the `_config.yml` file. The configuration file has many adjustable parameters to customize your site.

#### How do I add a favicon to my site?

Easy! Just place a valid `favicon.ico` (or another valid favicon image) in the root directory of your project. And then wait! It can take a while to update.

#### How do I move the blog to another page instead of having it on the home page?

The default style of Beautiful Jekyll is to feature the blog feed on the front page. But for many sites that's not the ideal structure, and you may want to have a separate dedicated page for the blog posts. To have the blog hosted on a different URL (for example at `<mysite.com>/blog`), copy the `index.html` file into a folder with the same name as the desired page (for example, to `blog/index.html`), and in the `_config.yml` file you need to add a parameter `paginate_path: "/<page name>/page:num/"` (for example `paginate_path: "/blog/page:num/"`).

#### What size do you recommend using for the `bigimg` photos?

Unfortunately, this is a no-answer! There isn't a one-size-fits-all solution to this, because every person will view your site on a different browser with different dimensions. Some browsers will have very wide aspect ratio, some will be narrower, some will be vertical (such as phones), different phones have different screens, etc. The image will always be centered, so the only tip I can give is that you should make sure the important part of the image is in the middle so that it'll always show. Other than that, every browser will show a different clipping of the image.

## Credits

This template was not made entirely from scratch. I would like to give special thanks to:
- [Barry Clark](https://github.com/barryclark) and his project [Jekyll Now](https://github.com/barryclark/jekyll-now), from whom I've taken several ideas and code snippets, as well as some documenation tips.
- [Iron Summit Media](https://github.com/IronSummitMedia) and their project [Bootstrap Clean Blog](https://github.com/IronSummitMedia/startbootstrap-clean-blog), from which I've used some design ideas and some of the templating code for posts and pagination.

I'd also like to thank [Dr. Jekyll's Themes](https://drjekyllthemes.github.io/), [Jekyll Themes](http://jekyllthemes.org/), and another [Jekyll Themes](http://jekyllrc.github.io/jekyllthemes/) for featuring Beautiful Jekyll in their Jekyll theme directories.

## Contributions

If you find anything wrong or would like to contribute in any way, feel free to create a pull request/open an issue/send me a message.  Any comments are welcome!

Thank you to [all contributors](https://github.com/daattali/beautiful-jekyll/graphs/contributors). Special thanks to  [@OCram85](https://github.com/OCram85) for contributing multiple times as well as helping with discussions.

If you do fork or clone this project to use as a template for your site, I would appreciate if you keep the link in the footer to this project.  I've noticed that several people who forked this repo removed the attribution and I would prefer to get the recognition if you do use this :)

## Known limitations

- If you have a project page and you want a custom 404 page, you must have a custom domain.  See https://help.github.com/articles/custom-404-pages/.  This means that if you have a regular User Page you can use the 404 page from this theme, but if it's a website for a specific repository, the 404 page will not be used.
"# stevearrants.github.io" 
