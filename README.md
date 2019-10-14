# Browse Beers and Save Your Favorite


## *Getting Started*
Start off by forking this repository into your own github profile. What you will specifically build out is detailed below. Commit as often as possible, we really enjoy seeing your work as it progresses!


## *Brief*
### 1. Create a simple webapp that uses React and Redux. This is a good method to begin the react part: https://github.com/facebook/create-react-app -- but use anything you are comfortable with!
### 2. This app should consist of two screens.
#### A. Page for browsing beer styles. The “beers” page will display a list of all beers, with a button that allows you to "favorite" any of them. 
#### B. The “favorites” page will show a list of all the beers that the user has favorited.


 ## *Details*
### Here is the API to use for this project: https://www.brewerydb.com/developers/docs 
#### You can register for a free developer account that allows for 10k calls per day. This should be more than enough!
##### Note: You should use the `.eslint` file included in this project to ensure that your code formatting is consistent with our practices. Look for linting plugins that support ESLint for whatever your text editior of choice is.

### Beers Page
#### The beers page will use the `/beers` endpoint, and should:
##### 1. Sort alphabetically (ascending + descending) by beer name. 
The API returns up to 50 results per page, so have your screen do the same, with a “load more results” button at the bottom that will request the next page of results and then slot them in under existing ones, without any kind of page reload. (https://www.brewerydb.com/developers/docs/endpoint/beer-index)

##### 2. Each beer entry will have a “favorite” button beside it, which will toggle whether or not that beer is a part of the user's list of favorite beers, STORED IN THE REDUX STATE. 

### Favorites Page
#### The favorites page will show a list of the beer names that the user has favorited. 
##### 1. A button alongside each should allow them to “unfavorite”. 
You only need to support one user, and they don't need to go through any kind of login process, so the user state will likely just consist of the list of their favorites.


### *Measurables*
1. At the conclusion of this project, you will have a locally-running application that we can clone on our machines and run locally ourselves in the same way.
 ##### Please provide any run instructions we will need inside your Readme.md

2. We’re interested in code quality and organization much more than a pretty appearance on the frontend ([s]css). So don’t worry about spending a lot of time styling things, a very basic look is all you need.

3. Use React, and Redux for state management. During requests to the beer API, the state should reflect that there is a request in progress, and should show some kind of loading bar on the front end.

##### Note: Spend time at the start of the project to plan things out. You want to make sure that you have exactly as many reducers and actions as it would make sense to use.


### *Bonus Section*
##### If you finish the above, and/or the above seems too trivial to you, build this with next.js!
Build this with [Next.js](https://nextjs.org), which handles routing and supports serverside rendering. This framework should be used in addition to React and Redux. They have nice tutorials [here](https://nextjs.org/learn/basics/getting-started). If you attempt this, you should make use of Next’s `getInitialProps()` lifecycle function to initially get the data for populating your state. Details about that function can be found here: https://nextjs.org/docs#fetching-data-and-component-lifecycle
###### Note: next.js is it's own beast! Be careful going this route, as seeing a working web app doing what is listed outside of this bonus section is the main goal.
