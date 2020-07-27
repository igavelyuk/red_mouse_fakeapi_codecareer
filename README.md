# Red mouse fakeapi
## CodeCareer.io
### User Settings test api

If you make POST, PUT, PATCH or DELETE requests, changes will be automatically and safely saved to db.json using lowdb.

## Basic fakeapi start from ground
[Project repo](https://github.com/typicode/json-server)
1. Install JSON Server global
`npm install -g json-server`
2. Create Folder, go in Folder
`yarn init`
3. Install JSON Server
`yarn add json-server`
4. Create a db.json file with some data
```JSON
{
  "userCredentials":
      {
        "displayname": "Igor Gavelyuk",
        "username": "igavelyuk",
        "email": "gavelyukworking@gmail.com",
        "phonenumber": "+380666540976",
        "lang": 0
      }
}
```
5. Edit `package.json`
```JSON
{
  "name": "red_mouse_fakeapi_codecareer",
  "version": "1.0.0",
  "description": "test-server",
  "main": "index.js",
  "repository": "https://github.com/igavelyuk/red_mouse_fakeapi_codecareer.git",
  "author": "igavelyuk <gavelyukworking@gmail.com>",
  "license": "MIT",
  "private": false,
  "dependencies": {
    "json-server": "^0.16.1"
  }
}
```
6. Add to `package.json`
```JSON
,
"scripts": {
  "json:server":"json-server --watch db.json"
}
```
7. Run `yarn run json:server`
```bash
yarn run v1.22.4
$ json-server --watch db.json

  \{^_^}/ hi!

  Loading db.json
  Done

  Resources
  http://localhost:3000/userCredentials

  Home
  http://localhost:3000

  Type s + enter at any time to create a snapshot of the database
  Watching...
```

#### version and date
`version-1.0.0`
`27 Jul 2020`
