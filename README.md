# Dinner App

### Goal of project

Main goal was to help to organize dinners ordering in out company. It allows user to pick particular dinner, choose if (s)he wants soup and then save it to data base. Admin user can block picks to avoid picking after order.

### Dependencies

Project is written in Javascript, fully in AngularJS. It using:
- bootstrap - gives application it's appearance
- ui-router - responsible of routing in app
- toaster - little notification library, showing user statuses
- chart.js - library for creating charts and plots, this allows to show data in graphical mode.

### Installation

Firstly, install packages by: `(sudo) npm install` and `bower install` (some packages are available only by bower).
If you want to run sass compiler, type: `gulp`. Backend of application is written in php, so if you want to run application locally, you need to run it through with for example `apache` and upload mysql database. For database conf file contact with application administrator.

#### Fake database

If you want to use fake db, you have to install json-server, by: `(sudo) npm install -g json-server`, run this fake server by: `json-server --watch fakedb.json` (file `fakedb.json` is included in project) then change part of `environmentSrv.js` file into:
```
        /* main database */
        // var apiBase = 'api/v1/';

        /* fake database */
        var apiBase = 'http://localhost:3000'
```
