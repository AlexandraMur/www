# AI Village website
[https://aivillage.org/](https://aivillage.org/)

# Blog

If you want to contribute a blog post just email blog@aivillage.org! We can help you edit it and tailor it to our audience. If you've just started writing or have an idea, email us and we'll do our best to help you get your content out there. We'll take [techical posts](https://aivillage.org/posts/dimensionality-and-adversarial/) and [non-technical ones](https://aivillage.org/posts/max-evil-sjterp/). We'll also take cross posted blogs and you can put your social media links at the top of the post. 

The final stage is just a zip with a markdown file, and a folder for the images, javascript, and pages you’d like to include. For an example, [this post](https://aivillage.org/posts/optimization-fgsm/) is generated by [this markdown](https://raw.githubusercontent.com/aivillage/www/code/content/posts/optimization-fgsm.md) with [this content folder](https://github.com/aivillage/www/tree/code/static/material/fgsm_images). We support Mathjax, and you can see examples of that in the included markdown in the zip. Currently javascript things like slideshows are done in iframes, we can help you get these working. If you have any questions or want to do something weird (like the toys here), just ask and we can figure something out.

# Info
This is a static website is generated with [Hugo](https://gohugo.io/) using the [Coder](https://github.com/luizdepra/hugo-coder/) theme. You will need hugo 0.40 or greater, which ubuntu 16.04 does not install by default. However, homebrew and later versions of ubuntu are fine. You will also need [lesscss](http://lesscss.org/) and [uglifycss](https://github.com/fmarcia/UglifyCSS) through node.

# Build & Deploy
The source code for the site is hosted on the ["code" branch](https://github.com/aivillage/www/tree/code) and static assets are served from the ["master" branch](https://github.com/aivillage/www/tree/master).

To make use of the `deploy.sh` script, your build environment should be organized as such:

```
root
|-- code (CURRENT DIRECTORY) -> tracking code branch of aivillage/www.git
|    +-- archetypes 
|    +-- content
|    +-- data
|    +-- ...
|    --- README.md
|    --- deploy.sh
|    --- ...
|-- site-assets -> tracking master branch of aivillage/www.git
|   +-- about
|   +-- categories
|   +-- css
|   +-- ...
```

To test that all the files are in the correct location and everything points correctly you can use `deploy_local.sh`. This will do all the steps in the normal deploy script, but not upload the result to github. 

For the local deployment, the links are all absolute and will point to the actual website, so static assets and links on your local site will not work. However it is useful for formating content.

# Contributors
Main developer of the site is [@cchio](https://github.com/cchio). Please contact him for any escalations or questions.