# Create-React-App-Travis
[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors)
A short number of steps to get a react app build, tested and then hosted on Github Pages using Travis.



### Steps:

#### Create React App
These steps assume you have NodeJS installed. You also need to install create-react-app. If you dont have this enter : 

```
npm install -g create-react-app
```

#### Homepage Setup

By default, React expects the page to be served from the root of a domain.
However, if the page is being served on GitHub Pages, it won't be there, so you need to tell React to use relative paths.

Edit your `package.json` as such:

```json
{
  "name": "...",
  "version": "...",
  "more fields": "...",
  
  "homepage": "."
}
```

#### Travis setup 
Travis needs to be setup to start builds when we push to the master. 

In order to run and build our content we dont need to provide travis with much other than a config file. But in order to give travis access to the repo to push builds we will need to generate a personal access token. 

#### Github Pages Setup

To set up github pages auto builds we need to give travis a personal access token. This can be gotten from [here](https://github.com/settings/tokens).

We we have the personal access token we need to set it up as an enviroment variable in Travis itself like so :  
![alt text](https://github.com/Ryan-Gordon/Create-React-App-Travis/blob/master/travis-settings.png)
  
![alt text](https://github.com/Ryan-Gordon/Create-React-App-Travis/blob/master/travis-env.png)


##### References
Inspired by this [ article](https://medium.com/@bezgachev/6-simple-steps-to-automatically-test-and-deploy-your-javascript-app-to-github-pages-c4c32a34bcb1)

## Contributors

Thanks goes to these wonderful people ([emoji key](https://github.com/kentcdodds/all-contributors#emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START -->
<!-- prettier-ignore -->
| [<img src="https://avatars1.githubusercontent.com/u/11082710?v=4" width="100px;"/><br /><sub><b>Ryan Gordon</b></sub>](https://github.com/Ryan-Gordon)<br />[💻](https://github.com/Ryan-Gordon/Create-React-App-Travis/Ryan-Gordon/Create-React-App-Travis/commits?author=Ryan-Gordon "Code") [📖](https://github.com/Ryan-Gordon/Create-React-App-Travis/Ryan-Gordon/Create-React-App-Travis/commits?author=Ryan-Gordon "Documentation") | [<img src="https://avatars0.githubusercontent.com/u/5843303?s=460&v=4" width="100px;"/><br /><sub><b>Zach Deibert</b></sub>](https://github.com/zachdeibert)<br />[📖](https://github.com/Ryan-Gordon/Create-React-App-Travis/Ryan-Gordon/Create-React-App-Travis/commits?author=zachdeibert "Documentation") |
| :---: | :---: |
<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the [all-contributors](https://github.com/kentcdodds/all-contributors) specification. Contributions of any kind welcome!