# hoodieshop
[How Hood.ie works](http://docs.hood.ie/en/latest/about/how-hoodie-works.html)
[Glossary](http://docs.hood.ie/en/latest/about/glossary.html)

### introduction
```
mkdir init
cd init
npm init
npm install hoodie --save
edit package.json >> scripts.start = "hoodie"
npm start
go to http://127.0.0.1:8080/hoodie/store/
open console 
type hoodie
yay!
some secrets http://127.0.0.1:8080/hoodie/admin/
```

```
add this to package.json
  "hoodie": {
    "address": "127.0.0.1",
    "port": 8080,
    "data": ".hoodie",
    "public": "public",
    "dbUrl": "",
    "dbAdapter": "pouchdb-adapter-fs",
    "inMemory": false,
    "loglevel": "warn",
    "url": "",
    "adminPassword": "secret"
  }
```
### configuration

http://docs.hood.ie/en/latest/guides/configuration.html

### demos

https://github.com/hoodiehq/hoodie-camp-tutorial
https://github.com/hoodiehq/hoodie-app-tracker

### Based on Hoodie

https://tracker.hood.ie/
https://minutes.io/welcome
https://github.com/hoodiehq/hoodie-app-mapchat

### plugins
[lot of plugins](https://www.npmjs.com/search?q=hoodie-plugin-)
