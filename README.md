# Create-React-App-Travis
A short number of steps to get a react app build, tested and then hosted on Github Pages using Travis.



### Steps:

#### Create React App
These steps assume you have NodeJS installed. You also need to install create-react-app. If you dont have this enter : 

```
npm install -g create-react-app
```

#### Travis setup 
Travis needs to be setup to start builds when we push to the master. 

In order to run and build our content we dont need to provide travis with much other than a config file. But in order to give travis access to the repo to push builds we will need to generate a personal access token. 

#### Github Pages Setup

To set up github pages auto builds we need to give travis a personal access token. This can be gotten from [here](https://github.com/settings/tokens).

We we have the personal access token we need to set it up as an enviroment variable in Travis itself like so :  
![alt text](https://raw.githubusercontent.com/Ryan-Gordon/Create-React-App-Travis/master/travis-settings.png)
  
![alt text](https://raw.githubusercontent.com/Ryan-Gordon/Create-React-App-Travis/master/travis-env.png)


##### References
Inspired by this [ article](https://medium.com/@bezgachev/6-simple-steps-to-automatically-test-and-deploy-your-javascript-app-to-github-pages-c4c32a34bcb1)
