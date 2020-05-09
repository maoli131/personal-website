# Personal Website

www.li-mao.net

## Introduction

This repository contains the source code of my personal website. My personal website serves as the central branding hub for myself. It includes my resume, showcases my portfolio, and references my other websites/social media.

Anything you want to know about me, you find on my website.

## Technology

Two years ago, in 2018, I used pure HTML/CSS to build the original version of my website. At that time, I had little knowledge about frontend dev and my coding style was bad. As a result, it wasn't quite extensible or maintainable.

Now as I'm graduating from UCSD, I decided to build my website from the ground up. I've explored many frontend stacks and frameworks. In particular, I'm quite inclined to use the trendy React.js as in my other projects. I like to reuse modular components so that I could easily update my page without much copying. Its dynamic rendering also looks cool. 

However, after careful consideration, I finally settled on Bootstrap 4, even in 2020. Here are a few reasons.
- STATIC: my website will largely be static. There will be minimum user interaction. React.js's extra overhead isn't neccessary for this type of task.
- SEO: it might be easier for search engine optimization if my server responds with the full document.
- EASY: I'm not a frontend designer. Bootstrap makes everything simple and straightforward, while also allowing full customization. 

As in two years ago, I will use AWS S3 and Cloudfront to deploy my website. If in the future I decide to add more advanced functionalities that require complex routing, I might switch to use Node.js or Flask as my backend server. 

## Development

I used `gulp` to automate the build process and `npm` to manage `gulp` and other javascript library dependencies. `gulp` also enables me to use HTML partials as resusable components. 
```
$ npm install
$ gulp
```

To build the production files, run the following:
```
$ gulp build
```
The production files will be in the `dist/` folder. 