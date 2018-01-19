# Rails 5.0 API and React Front-End
Running both servers
```
rake start
```
Testing production
```
rake start:production
```
Explanation of rake task
- foreman will start the front end
- /client, on port 3000 and the API on port 3001. 
- It’ll then open the client http://localhost:3000 in your browser.
- You can access ActiveAdmin via the API, at http://localhost:3001/admin

### Production Setup Details
- Uses heroku
- Had to use heroku's buildpaclks to execute node code first before Rails
- Set up procfile specifically for production
- Since `create-react-app` defines react-scripts as devDependency in client/package.json
  - need to set NPM_CONFIG_PRODUCTION to false so that the build won't disregard devDependencies in our case, devDepencies was not creation so we didn't need to do this
- 


### Sources
- Original guide
  - https://medium.com/superhighfives/a-top-shelf-web-stack-rails-5-api-activeadmin-create-react-app-de5481b7ec0b