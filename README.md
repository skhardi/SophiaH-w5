# w5-Node
Bringing JavaScript to the backend.

# About
With Node.JS, we're now in the backend. We're getting closer and closer to full-stack - it's just right around the corner.

Node.JS is an open-source runtime environment introduced in 2009, built upon Chromium V8 - made by Google for Chrome and written in C++. Practically speaking, before Node, web developers had to learn separate languages to develop in the backend - such as PHP. Node and its incredibly large package library allows us to write plain JavaScript to access databases, build our own APIs, and also allows us access to highly optimized and sophisticated front-end tech such as React, and even mobile app development. On top of this, Node is lightweight and lightning-fast, with companies such as PayPal reporting over 35% quicker response time and ability to handle double the amount of requests-per-second compared to pre-Node tech stacks.

Here's a comparison of a couple performance metrics between Node and the Apache (Java)/PHP stack that is seen in the now uncommon, but oft-utilized LAMP stack - the classic industry standard of web development.

![](https://res.cloudinary.com/practicaldev/image/fetch/s--VqEadoeX--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://raw.githubusercontent.com/emilioSp/node-vs-apache/master/results/graphs/Simulated%2520IO%2520time%2520per%2520request.svg)

![](https://res.cloudinary.com/practicaldev/image/fetch/s--ivW2_-MA--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://raw.githubusercontent.com/emilioSp/node-vs-apache/master/results/graphs/CPU%2520intensive%2520time%2520per%2520request.svg)

![](https://res.cloudinary.com/practicaldev/image/fetch/s--Dvjq_Zky--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://raw.githubusercontent.com/emilioSp/node-vs-apache/master/results/graphs/Simulated%2520IO%2520requests%2520per%2520second.svg)

And as I said, we won't have to learn any new languages - we're going to be doing just about everything with the exact same syntax and coding conventions as we've been using so far in the front-end. No switching between Java, PHP, Ruby, .NET - just JavaScript all the way through. 

For these reasons, tech stacks utilizing Node are by far and away the most popular in the industry, seen most commonly paired with Angular and React (MEAN/MERN), the latter of which we'll be using.

# Quick start commands and NPM
Refer to the previously-posted download links for Node to install - contact me if you have any questions.

Packages are another big thing that sets Node apart - essentially importing of other libraries, functions, etc. and Node has one of the absolute biggest package libraries imaginable.

Packages are handled by NPM (Node Package Manager), and are stored exclusively on the client-side once installed so we don't have to be uploading and using hosting to store our files. Our package.json and .gitignore files are how we do this.

Take a look at this repository's contents - you'll find the package.json and package-lock.json, but nothing else regarding Node modules. These two files contain the information about the Node packages the repo uses. If you were to run ```npm i``` (shorthand for ```npm install```), it would automatically install the package Inquirer which you'd find in your newly created node_modules folder, which is a folder I have on the local repository, but not on the GitHub-hosted repository.

You'd also notice some 700+ file changes in your VSCode source control UI on the left-hand side. To avoid uploading the actual node_modules folder, we simply use a .gitignore file with the files we DON'T want pushed to GitHub. This file is also in the repo, and it's a lot simpler than you think. It's essentially a blank text file with the names of the files/folders we don't want - in our case, node_modules. We'll be adding this .gitignore in every single Node project we do.

If you're wondering, you *cannot* gitignore the .gitignore. We have to add a global gitignore for that one :)

# Activities
7/13: For today, just verify all of our software is set up and running so we can work out those kinks early. 

* Clone down this Node repository

* Copy all of the files into your own repository.

* Run ```npm i``` in your own repo. It should download a fair bit of node_modules.

* Verify node_modules is in the .gitignore, and push up the repository.

* If your repository DIDN'T upload your node_modules folder, you're good to go.

Once you're done, go ahead an explore the Node environment. Try running various Node commands, and create a JS file with some basic console.logs to see what our development practice is going to look like now. Feel free to create some basic functions and algorithms and log them to see how they're compiled in Node. Once you've written some code in your JS file, you can execute it with ```node myFile.js```.

If you're ever creating a live process, you can always terminate a Node program with ```CTRL + C```. This is how we close hosted servers as well.

They also have some really good documentation to give a quick glance around - but if nothing else, take a look at this page. It may make your lives so much easier in the future. Task coming tomorrow (7/14).

https://nodejs.dev/learn/how-to-log-an-object-in-nodejs