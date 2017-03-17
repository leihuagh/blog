---
title: Getting Start Angular 2 (01)
tags:
  - angular2
  - angular2_heroes
categroies: tutorials
date: 2017-03-17 14:28:46
categories:
---


### Step 1. Set up the Development Environment

In my case, I would like to choose @angular/cli, install @agnular/cli into your computer globally.

``` bash 
npm install -g @angular/cli
```

### Step 2. Create a new project

- Open Git bash terminal under "C:\projects\"
- Generate a new project and skeleton application by running the following commands:

``` bash
ng new my-app
```

### Step 3: Serve the application

Go to the project directory and launch the server

``` bash
cd serve --open
``` 

- The `ng serve` command launches the server, watches your files, and rebuilds the app as you make changes to those files 
- Using the `--open` (or just `-o`) option will automatically open your browser on http://localhost:4200/
- Your app greets you with a message:

![App Works](./images/angular2/heroes/app-works.png)



