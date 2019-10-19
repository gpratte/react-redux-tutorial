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

Removed all the default files and edited the remaining files to just show an html page with an h1 header. The files are now
* index.js
* index.css
* App.js

Push the changes
* _git add ._
* _git commit -m "the app just shows an h1 header"_
* _git push origin master_

Edit the README.md with these notes and push changes to master.
* _git add ._
* _git commit -m "update readme"_
* _git push origin master_

Create the first branch
* _git checkout -b step-01-create-development-environment_
* _git push origin step-01-create-development-environment_

## step 02 actions
Created a **step-02-actions** branch from master

Read through the https://redux.js.org/basics/actions page of the basic tutorial.

Added (copied and paste) the actions.js file, pushed the branch and then merge the branch to master.

## step 03 reducers
Created a **step-03-reducers** branch from master

Read through the https://redux.js.org/basics/reducers page of the basic tutorial.

Added (copied and paste) the reducers.js file, pushed the branch and then merge the branch to master.


## step 04 store
Created a **step-04-store** branch from master

Read through the https://redux.js.org/basics/store page of the basic tutorial.

Updated (copied and paste) the index.js file with
```
import { createStore } from 'redux'
import todoApp from './reducers'
const store = createStore(todoApp)
```

Tried to run the app
* _npm start_

and it complained it did not know what redux is so install redux
* _npm install --save redux_

and the app ran with no problems.

Pushed the branch and then merge the branch to master.


## step 05 presentational components
Created a **step-05-presentational-components** branch from master

Started working through the https://redux.js.org/basics/usage-with-react page of the basic tutorial.

This branch represents the Implementing Presentational Components section.

Create a **components** directory.

Copied (cut and paste) into the Todo.js file.

Copied (cut and paste) into the TodoList.js file.

Copied (cut and paste) into the Link.js file.

Copied (cut and paste) into the Footer.js file.

Ran the app and it did not report any problems.
* _npm start_

I am surprised because Footer imports FilterLink which does not exist.

```
import FilterLink from '../containers/FilterLink'
```

Pushed the branch and then merge the branch to master.

## step 06 container components
Created a **step-06-container-components** branch from master

Continued working through the https://redux.js.org/basics/usage-with-react page of the basic tutorial.

This branch represents the Implementing Container Components section.

Create a **containers** directory.

Copied (cut and paste) into the FilterLink.js file.

Copied (cut and paste) into the VisibleTodoList.js file.

Pushed the branch and then merge the branch to master.


## step 07 implementing other components
Created a **step-07-implementing-other-components** branch from master

Continued working through the https://redux.js.org/basics/usage-with-react page of the basic tutorial.

This branch represents the Implementing Other Components section.

Copied (cut and paste) into the AddTodo.js file.

Copied (cut and paste) into the components/App.js file.

Yes there is an App.js in the src directory and another in src/components directory.
index.js still uses the first one.