---
title: Getting Start with Hexo Blog
date: 2017-03-17 9:56:02
tag: hexo
---

### Requirements
Installing Hexo is quite easy. However, you do need to have a couple of other things installed first:

*   Install [Node.js](https://nodejs.org/en/). Download right side one.
*   Install [Git](https://git-scm.com/). Download the latest version

### Installation Process

1. Create a "projects" folder under your C:\
2. In Windows Explorer, Navigate the "C:\projects"
3. Highlight "projects", right-click to bring pulldown menu, select "Git Bash Here" to open the git bash.
4. Do install Hexo into your computer by following the codes below

``` bash
$ npm install -g hexo-cli
```

### Initializatng a blog

``` bash
$ hexo init blog
$ cd blog
```

### Editing the Overall Configuration File

#### Turn on the server in watch to watch the changes

``` bash
$ hexo server --watch
```

#### Config the site general information

1. I am using Visual Studio Code 
2. Open "C:\projects\blog\" folder in VS Code 
3. Open "_config.yml" file under blog root directory
4. Customize the site general settings by your info.  Below are my settings

``` bash
title: 迷彩网后博客园
subtitle: 网阔凭余跃, 云高任偶飞
description: This is my GitHub blog home
author: Lei Hua
language:   
  - en
  - zh-cn
  - zh-tw
timezone: America/New_York
```

#### Config the deployment information
5. Customize deployment info on your side.  Below are the sample of mine

``` bash
deploy:
  type: git
  repo: https://github.com/leihuagh/leihuagh.github.io.git
  branch: master 
```

### Deploy to remote sites

If you think the http://localhost:4000 results are what you want, the next step is delopy them into GitHub 

#### Create a repository on your GitHub account 

- Go to your GitHub home to create a new repository
- In my case, I created a repository called "leihuagh.github.io"

#### Generate the static HTML files 

Run the code below to generate all of the HTML files into a generated folder called "public"

``` bash
$ hexo generate
```

After executing generate command, the new folder called "public", which contains all of the site files, will be generated

#### init git in public

``` bash
$ cd public 
$ git init
$ git add --all 
$ git commit -m "Initializing blog"
$ git status
```

#### Public the contents to GitHub

Now, I am ready to send all of the folders and files under public folder to GitHub repository

``` bash
$ git remote add origin https://github.com/leihuagh/leihuagh.github.io.git
$ git push origin master
```
If git push command gets failure, you can add option: --force

``` bash
$ git push origin --force
```

#### View Your GitHub Glog home

Open your browser and access https://<your github account name>.github.io/




