# Musilinky: 
A website I contributed to as part of a team during my time at CU Boulder. The website implements a search engine that allows users to search for a song and receive results for the song's URL on different music streaming services.

The website is comprised of several webpages containing CSS formating and Javascript, EJS for UI and NodeJS for server interactions.

The MusicAPI, DuckDuckGo API, Deezer API, and Soundcloud Downloader API are all used for the website's functionality.

An SQL database is implemented for storing user info.

**Testing**  
Testing is handled with Mocha and Chai, to run the tests the following can be copied into the package.json file:
```
{
  "name": "project-3308",
  "main": "index.js",
  "dependencies": {
    "ejs": "^3.1.8",
    "ejs-lint": "^0.3.0",
    "express": "^4.6.1",
    "pg-promise": "^10.11.1",
    "body-parser": "1.20.0",
    "express-session": "1.17.3",
    "bcrypt": "^5.1.0",
    "axios": "^1.1.3"
  },
  "devDependencies": {
    "nodemon": "^2.0.7",
    "chai": "^4.2.0",
    "chai-http": "^4.3.0",
    "mocha": "^6.2.2",
    "npm-run-all": "^4.1.5"
  },
  "scripts": {
    "prestart": "npm install",
    "start": "node index.js",
    "dev": "nodemon server.js",
    "test": "mocha",
    "testandrun": "npm run prestart && npm run test"
  }
}
```
Then, change the command in the bottom of the docker compose file to 'npm run testandrun'.

**Credits**  
Alex Burch  
Silas Khan  
Eric Gosnell  
Patrick Fleming  
Tyler Chung  
Cade Williams  
