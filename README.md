# Friend Finder

### Details on the assignment
This is the creation of a compatibility-based "FriendFinder" application -- basically a dating app. This full-stack site will take in results from the users' surveys, then compare their answers with those from other users. The app will then display the name and picture of the user with the best overall match. 

### Why use express.js?
Express.js is a framework used for Node and it is most commonly used as a web application for node js. Express is just a module framework for Node that you can use for applications that are based on server/s that will "listen" for any input/connection requests from clients. Node.js and Express.js are a perfect match. Express is a fast, minimalist framework that sits on top of Node.js and allows you to build powerful single- and multi-page web applications and websites.

### How you create the webpage

We use Express to handle routing and deploy the app to Heroku so other users can fill it out. The survey has 10 questions with each answer on a scale of 1 to 5 based on how much the user agrees or disagrees with a question. The most compatible friend will be found by following as a guide: 

* Convert each user's results into a simple array of numbers (ex: `[5, 1, 4, 4, 5, 1, 2, 5, 4, 1]`).
   * With that done, compare the difference between current user's scores against those from other users, question by question. Add up the differences to calculate the `totalDifference`.
     * Example: 
       * User 1: `[5, 1, 4, 4, 5, 1, 2, 5, 4, 1]`
       * User 2: `[3, 2, 6, 4, 5, 1, 2, 5, 4, 1]`
       * Total Difference: **2 + 1 + 2 =** **_5_**
   * The absolute value of the differences will be used. Put another way: no negative solutions! The app should calculate both `5-3` and `3-5` as `2`, and so on. 
   * The closest match will be the user with the least amount of difference who will show as a modal pop-up which will show his/her name and picture

## Technologies used

* node.js

* express.js

* npm packages: express, body-parser, path

### Ending Notes

There were many examples of similar projects found on Github, Stack Overflow, W3 Schools, the Firebase website which you could use as reference. However just googling certain parts that you are stuck on help as well. (Google Fu!) Also, turning to your classmates helps a great deal. I learned that just by talking it out with classmates, often times you are able to answer your questions yourself!

Fill out the survey and find your best match!