# vercel-express

Vercel Express and UI Webapp Example.

Live Demo - https://bottleproject.vercel.app/

# Mongodb
The application is able to connect to mongodb. The code is in db.js

### Set up & Deploy with Vercel

```
$ npm install vercel -g
$ npm install
$ vercel
```

### To run on localhost
Sign up for an account on [vercel](https://vercel.com)

Run the following command:
```
$ vercel login
```

You should be asked for your email. Type in your email and proceed to your email inbox.
After you have logged in select the relevant project. You can just press enter if there is only one project.
After you have setup everythign and logged in, run the following command and then it will tell you which port it is running at

```
$ vercel dev
```

### To use graphQL server
After you run the application navigate to http://localhost:3000/api/



- Vercel will generate a ".vercel" directory, don't share or commit this one.
- After deploying, open your URL like this:
  - http://YOUR-VERCEL-APP-ID.vercel.app
  - Example: https://vercel-express-3.ngduc.vercel.app

### [app/index.js](./app/index.js)

- If you're using Typescript, build your source directory, output to "app"
- Update package.json: "main": "app/index.js"

### [vercel.json](./vercel.json)

- Map API routes (/api/...) and static (UI) routes (/...).
- Environment variables - examples:
  - ```$ vercel secrets add my-mongodb-uri mongodb+srv://<user>:<password>@clusteridxxx.mongodb.net/<database-name>?retryWrites=true```
  - add "env" to vercel.json ```{ "env": { "MONGODB_URI": "@my-mongodb-uri" }, ... }```


### Links
- https://vercel.com/guides/using-express-with-vercel
- https://medium.com/javascript-in-plain-english/create-and-deploy-a-node-js-express-app-for-free-f75d8796ba70
- https://www.apollographql.com/docs/apollo-server/getting-started/
