---
title: Working with Images
tags: hexo
categories: tutorials
date: 2017-03-17 12:47:08
---


### Create the Post with Images

A good practice when starting new posts is to use the "draft" feature. Drafts will not be published by default, so you are free to make changes to other posts while keeping unfinished drafts hidden from public.

``` bash
$ hexo new draft "working-with-images"
# creates -> ./source/_drafts/working-with-images.md
```

### Inserting images

Images and other asset files can be placed in subdirectories under the ./source/ folder. Use a picture downloaded from google images. In my case, I use Hexo logo. Download the picture into the path below,

``` bash
./source/_images/hexo_logo.png
```

### Adding Image Link to Draft File 

Edit your draft by adding the code below

``` bash
![Hexo Logo](./images/hexo_logo.png)
```

![Hexo Logo](./images/hexo_logo.png)

### Publishing Drafts

When it's time to move the draft to a "live" post for the world to see, use the hexo publish command:

``` bash
$ hexo publish working-with-images
```

A few things will happen when this command is run:

- The markdown file My-First-Blog-Post.md moves from ./source/_drafts/ to ./source/_posts.
- The file's "front-matter" changes to include a publish date:

### Generate the Static File

Finally, prepare the entire site for deployment. Run the hexo generate command:

``` bash
$ hexo generate 
# generates -> ./public/
```

### Next Steps

- Update gitHub repository 
- Detail way refer to Getting Start Page