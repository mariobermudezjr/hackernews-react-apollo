# React + Apollo Tutorial - Introduction

###### WRITTEN BY

![alt text](https://pbs.twimg.com/profile_images/938876572802650112/owTdBnzU_200x200.jpg 'Nikolas Burk')

###### Nikolas Burk - Developer @ Prisma

###### Nikolas is a developer and head of content at Prisma. He is excited about GraphQL as a new API technology and has a passion for learning and sharing knowledge.

## Overview

In the previous tutorials, you learned about major concepts and benefits of GraphQL. Now is the time to get your hands dirty and start out with an actual project!

You’re going to build a simple clone of Hackernews. Here’s a list of the features the app will have:

- Display a list of links
- Search the list of links
- Users can authenticate
- Authenticated users can create new links
- Authenticated users can upvote links (one vote per link and user)
- Realtime updates when other users upvote a link or create a new one

#### In this track, you’ll use the following technologies for building the app:

- Frontend:

  - React: Frontend framework for building user interfaces

  - Apollo Client 2.1: Production-ready, caching GraphQL client

- Backend:

  - graphql-yoga: Fully-featured GraphQL Server with focus on easy setup, performance & great developer experience

  - Prisma: Open-source GraphQL API layer that turns your database into a GraphQL API

You’ll create the React project with create-react-app, a popular command-line tool that gives you a blank project with all required build configuration already setup.

#### Why a GraphQL Client?

In the Clients section in the GraphQL part, we already covered the responsibilities of a GraphQL client on a higher level, now it’s time to get more concrete.

In short, you should use a GraphQL client for tasks that are repetitive and agnostic to the app you’re building. For example, being able to send queries and mutations without having to worry about lower-level networking details or maintaining a local cache. This is functionality you’ll want in any frontend application that’s talking to a GraphQL server - why build it yourself when you can use one of the amazing GraphQL clients out there?

There are a few GraphQL client libraries available. For very simple use cases (such as writing scripts), graphql-request might already be enough for your needs. However, chances are that you’re writing a somewhat larger application where you want to benefit from caching, optimistic UI updates and other handy features. In these cases, you have the choice between Apollo Client and Relay.

#### Apollo vs Relay

The most common question heard from people that are getting started with GraphQL on the frontend is which GraphQL client they should use. We’ll try to provide a few hints that’ll help you decide which of these clients is the right one for your next project!

Relay is Facebook’s homegrown GraphQL client that they open-sourced alongside GraphQL in 2015. It incorporates all the learnings that Facebook gathered since they started using GraphQL in 2012. Relay is heavily optimized for performance and tries to reduce network traffic where possible. An interesting side-note is that Relay itself actually started out as a routing framework that eventually got combined with data loading responsibilities. It thus evolved into a powerful data management solution that can be used in JavaScript apps to interface with GraphQL APIs.

The performance benefits of Relay come at the cost of a notable learning curve. Relay is a pretty complex framework and understanding all its bits and pieces does require some time to really get into it. The overall situation in that respect has improved with the release of the 1.0 version, called Relay Modern, but if you’re for something to just get started with GraphQL, Relay might not be the right choice just yet.

Apollo Client is a community-driven effort to build an easy-to-understand, flexible and powerful GraphQL client. Apollo has the ambition to build one library for every major development platform that people use to build web and mobile applications. Right now there is a JavaScript client with bindings for popular frameworks like React, Angular, Ember or Vue as well as early versions of iOS and Android clients. Apollo is production-ready and has handy features like caching, optimistic UI, subscription support and many more.

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br>
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.<br>
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.<br>
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br>
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (Webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: https://facebook.github.io/create-react-app/docs/code-splitting

### Analyzing the Bundle Size

This section has moved here: https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size

### Making a Progressive Web App

This section has moved here: https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app

### Advanced Configuration

This section has moved here: https://facebook.github.io/create-react-app/docs/advanced-configuration

### Deployment

This section has moved here: https://facebook.github.io/create-react-app/docs/deployment

### `npm run build` fails to minify

This section has moved here: https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify
