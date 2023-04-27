# Node Express CRUD - Starter CRUD from Brian Jenney JS Code 

This starter CRUD is just a jumping off point for understanding all the moving parts of a Node Express CRUD. There is not solution or tutorial for this project. This is a functional CRUD that can be incoroprated into other projects. For support and to work thru questions there is a private Slack community,  called JS CodeCoach, comprised of other bootcamp graduates and junior JavaScript/React developers whom are all working on strengthing their developer skills. This community is facilitated by [Brian Jenney](https://www.yourcodecoach.com/blog).

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Resources](#resouces)
- [My process](#my-process)
  - [What I learned](#what-i-learned)
- [Author](#author)


## Overview

### The challenge
The challenge is to learn as much as I can about how this CRUD works. This means breaking things and then fixing them. It means learning as much about each part of the code and finding good resources that I can use in the future. Its all about learning on my own, at my pace, and without a tutorial. This CRUD can also be used in future projects!🚀


### Resouces
- [Nodemon](https://www.digitalocean.com/community/tutorials/workflow-nodemon) - enables hot reloading
- Postman [Community Forum](https://community.postman.com/)

## My process
- Cloned and made git repo for this CRUD. Initially I had forked and cloned Brian's repo but I want this to be my own repo and claim those contribution boxes on Github ✅✅✅
- Using node.js version 18.16.0 and npm 9.5.1. I had installed nvm as a Node version manager a couple of days before and used ```nvm install --lts``` to get the latest long term support version of Node.js. 
- Changed the local port from 5000 to 3000. My Mac uses port 5000 for Airplay whatever that is??? I could only find one place to change this in the server.js file.
- This CRUD includes Nodemon script which allows for "hot reloading". Use ```npm run dev``` instead of ```npm start```. This is similar to what I have in my Catch of the Day project and in all my 11ty projects.
- The server.js file is listed in the package.json as the ``` "main": "server.js" ```. This means that this is the file excuted when you run npm start. This could easily be index.js or app.js. Similar to how in codesandbox.io when you hover over files you can find the entry file.
- Decided to use Postman API platform with this project. That took a little bit of doing to figure out. I even made a little [loom video](https://www.loom.com/share/8a0b04475bcc4fd8b05b89f0e597c427) about some of my confusion 😀


### server.js 
This file is executed when launch the CRUD. Notable bits in this file.
- Everything imported/define at the top is a node_module except for allRoutes. This points to the routes/index.js file.
- The server is where I changed the port from 5000 to 3000 for the local host listening
- I can't find an .env file???
- 

### userRoutes.js
This file defines what the CRUD is listening for. For example if you want to add a user then you would type ``` http://localhost:3000/user/``` and then use [post]. This is defined in the first line in the code below.
``` 
router.route('/').post(validateUserBody, createUser);
router.route('/:id').get(validateUserBody, getUser);
router.route('/').put(validateUserBody, updateUser);
router.route('/:id').delete(validateUserBody, removeUser);
```



### What I learned


## Author

- Website - [Amy Spencer](https://spencerproject.com/)
- Frontend Mentor - [@amyspencerproject](https://www.frontendmentor.io/profile/amyspencerproject)
- Linkedin - [amyspencercodes](https://www.linkedin.com/in/amyspencercodes/)