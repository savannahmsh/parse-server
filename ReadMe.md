## Configuration Steps
  - Install mongodb and create a database `intelehealth_images`
  - Install node.js `npm install -g npm@4.6.1`
  ```sh
  $ npm install -g npm@4.6.1
  $ npm install -g parse-server
  $ npm install -g mongodb-runner
  $ mongodb-runner start
$ npm install -g parse-dashboard
$ npm install pm2@latest -g
  ```
  - Create parse dashboard config on your current working directory `nano PARSE_DASHBOARD_CONFIG.json`. Replace it with the contents of the file `PARSE_DASHBOARD_CONFIG.json` from this repository.
  Make sure to update the serverIP and add the necessary users.

 - Create a config file `nano FILENAME.json` and copy the corresponding content of the file from this repository.
 
 ```sh
$ pm2 start FILENAME.json
$ pm2 status
```
