# Build and Deployment notes

## Pre-build

Once you have done your commit on your branch and you've finished the feature you're working on, merge your changes into the master branch following these steps:
- Navigate to repository at [your github repository](https://github.com/gerritbutler/gerritbutler.github.io/)
- click [Pull Requests](https://github.com/gerritbutler/gerritbutler.github.io/pulls)
- You should see your branch there with a button that says "Compare & pull request"
  - note: if you don't see your branch, make sure you pushed it up from your local machine

## Build

We want to now build the project and put all of the goodies into the dist folder. Basically, it deletes all of the contents of the dist folder and copies the files from the src directory instead. But first, it copies the index.html into the src folder before wiping directory. 

You will see several build files running, it is basically just shuffling files around to prepare for the deploy command. 

type the following command in your terminal: `npm run build`

## Deploy

Next we need to deploy our changes to gh pages. This deploy command has some logic that will do the deployment to your website. 

type the following command in your terminal: `npm run deploy`