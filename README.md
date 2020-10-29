# Create Social Network

Create Social Network is a educational project. The main idea is to demonstrate how one can build a large scalable project with Javascript. However you get the core functionality of social network by running one command and then you can build more on top of that.

Repository is divided into three main packages:

- **api** This package contains API for Social Networking App, built with Nodejs, Express, GraphQL, Apollo Server and MongoDB with Mongoose.
- **frontend** Is a frontend for Social Networking App, built with React, GraphQL, Apollo Client and Styled Components.
- **lib** Is a Nodejs command line script, that helps users to install the Social Networking App with one command. This package is published to NPM as a `create-social-network`

## Features

- **Messenger** Real time messaging system.
- **Notifications** Get instant notification when someone follows/messages you or likes/comments on your post.
- **User Status** Check if user is Online or not in real time.
- **News Feed** Fresh posts from people you are following.
- **Explore** New Posts and People.
- **Follow** a particular user and get notified for their activity.
- **Personalize Profile** With profile/cover photo and personal posts.
- **Authentication & Authorization** with Password reset functionality.

## Requirements and Configuration

You’ll need to have Node 8.16.0 or Node 10.16.0 or later version on your local development machine

By default, the app uses MongoDB hosted on [mLab](https://mlab.com/) and [Cloudinary](https://cloudinary.com/) CDN for hosting images. We have created a demo user for mLab and Cloudinary so you can run the app locally without adding Mongo URL and Cloudinary API Key, however when you start developing your application it is recommended to replace that information with your own, so that everyone has their own Database and CDN.

> Note demo database is being deleted and populated with demo data daily

### Replacing Mongo URL

Replace `MONGO_URL` value in `api/.env` file with your `mLab` database url or with local one.

### Replacing Cloudinary API Key

Grab `Cloud name` `API Key` and `API Secret` from Cloudinary dashboard and replace corresponding values inside `api/.env` file.

### Mail Provider

For password reset functionality you will need to replace Email Provider values also in `api/.env` file.

## Creating an App

### npm

```sh
npm install
```

### Yarn

```sh
yarn install
```

Once the installation is done, start the application with `npm start` or `yarn start` that will run the app in development mode.
Open [http://localhost:3000/](http://localhost:3000/) to view it in the browser.

The page will automatically reload if you make changes to the code.
