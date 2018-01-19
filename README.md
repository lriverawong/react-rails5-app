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

### Sources
- Original guide
  - https://medium.com/superhighfives/a-top-shelf-web-stack-rails-5-api-activeadmin-create-react-app-de5481b7ec0b