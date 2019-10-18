My First React/Redux Application

I've worked through the Redux Basic Tutorial (https://redux.js.org/basics/basic-tutorial).

The following shows what I did step by step.

Each step can be found on the cooresponding branch.

## step 01 create development environment
To get started did the following.

From https://reactjs.org/docs/create-a-new-react-app.html#create-react-app

* _npx create-react-app react-redux-tutorial_
* _cd react-redux-tutorial_

Removed the .git directory
* _rm -rf .git_

Created github repository react-redux-tutorial
Hooked up react-redux-tutorial with the github repository

* _git init_
* _git add ._
* _git commit -m "initial commit"_
* _git remote add origin https://github.com/gpratte/react-redux-tutorial.git_
* _git push origin master_

Make sure the initial react application works. Run
* _npm start_

should see the default react page in the web browser at http://localhost:3000/

From the redux tutorial "Usage with React" https://redux.js.org/basics/usage-with-react install react-redux
* _npm install --save react-redux_

Push changes
* _git add ._
* _git commit -m "added react-redux npm package"_
* _git push origin master_


Edit the README.md with these notes and push changes to master.
* _git add ._
* _git commit -m "update readme"_
* _git push origin master_

Create the first branch
* _git checkout -b step-01-create-development-environment_
* _git push origin step-01-create-development-environment_

