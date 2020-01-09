# Assignment 0:  Typescript, Web, Babylon warmup 

This is a skeleton, based on some of the Babylon examples, of a small project that will let you build, debug, and run Babylon applications locally.

The objective of this assignment is two-fold:
1. Get your computer set up to work with the toolset we are using.
2. Do a little bit of work with Babylon.

## Due: Friday Jan 17th, 11:59pm

## Name and GT user-id

Name: 
User ID:

## Rubric

Graded out of 10.

Each of the parts to be added are discussed in one of the lessons in the [Babylon 101](https://doc.babylonjs.com/babylon101/) tutorial.

0. Ensure your program builds with no Typescript warnings. (1)
1. Use the Universal camera to support movement in the scene.  (1)
2. Add a ground plane with some interesting ground texture.  Should be centered under the initial position of the camera. (1)
3. Change the PointLight that is in the sample code to a directional light that is not very bright and not white, and also add one SpotLight to the scene, a reasonable distance above the viewer's initial position. (1)
4. Add at least 5 objects, with interesting materials and/or textures, sitting on the ground. (1)
5. Use keyframe animation to add at least 2 moving objects above the initial viewer position, but below the lights. (1)
6. When you click on one of your objects with the mouse, play a sound and have a particle system shoot particles out from the center of the object. (1)
7. Add shadows, for both the directional and spot lights. (1)

2 additional points will be given for using interesting textures, lights and materials.  (You won't be judged on aesthetics;  I want you to do more than just cut and paste code and textures from the tutorial.)

## Overview 

The goal of the assignment is to get you up and running with doing Typescript and Babylon development on your machine. That's the main goal: you will get some initial experience with Typescript, and Babylon.

# Submission

You will check out the project from github classroom, and submit it there.  The project folder should contain just the additions to the sample project that are needed to implement the project.  Do not add extra files, and do not remove the .gitignore file (we do not want the "node_modules" directory in your repository.)

**Do Not Change the names** of the existing files (e.g., index.html, app.ts, etc).  The TAs need to be able to test your program as follows:

1. cd into the directory and run ```npm install```
2. start a local web server and compile by running ```npm run start``` and pointing the browser at your ```index.html```

Please test that your submission meets these requirements.  For example, after you check in your final version of the assignment to github, check it out again to a new directory and make sure everything builds and runs correctly.
 
# Development Environment

The sample has already been set up with a complete project for Typescript development.

To work with this sample and prepare your submission, you should have Node (and in particular, npm and npx) installed, which you can retrieve from [nodejs.org](http://nodejs.org).   

In addition to node, you should make sure a recent (e.g., version 3.7 or later) version of Typescript is installed, as described at [www.typescriptlang.org](http://www.typescriptlang.org).

Finally, we will use the node `npx` command to both build the project (with webpack) and run a local http webserver on your machine.  The ```package.json``` is set up to run this server 

## Running 

You set up the initial project by pulling the dependencies from npm with 
```
npm install
```

After that, you can compile and run a server with:
```
npm run start
```

You do not have to run ```tsc``` to build the .js files from the .ts files;  ```npx``` builds them on the fly as part of running webpack.

You can run the sample by pointing your web browser at ```https://localhost:8080/index.html```