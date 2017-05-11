# hoodieshop
[How Hood.ie works](http://docs.hood.ie/en/latest/about/how-hoodie-works.html)
[Glossary](http://docs.hood.ie/en/latest/about/glossary.html)

### Hoodie-Camp-Tutorial
```
git clone https://github.com/hoodiehq/hoodie-camp-tutorial.git
cd hoodie-camp-tutorial
npm install
npm start
```
#### notes
```
By default, every 30 secs check for availability of hoodie server
hoodie.connectionStatus.startChecking()
manual, events disconnect & reconnect
hoodie.connectionStatus.check()

hoodie.store.db
hoodie.ready

Colors

hoodie.store.add({name: 'pink'})
hoodie.store.findAll().then(console.table)
hoodie.store.findAll().then(console.dir)

hoodie.store.add({name: prompt('Enter color')})
hoodie.store.update(prompt('id'), {name: prompt('color')} )

hoodie.store.updateAll({name: 'beige'})
hoodie.store.remove(prompt('id'))

hoodie.store.update({_id: '8AC219A6-312C-0F8E-AC0D-1CEE73D84D50', name: 'red'})
hoodie.store.remove({_id: '8AC219A6-312C-0F8E-AC0D-1CEE73D84D50'})
```

### write your own hoodie app
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

Want to see something fun? Open this page in another browser, sign in with the same account, then add colors. Watch the magic happen…

Now turn of your internet connection. Add colors to both browsers. Turn on your internet connection again, and wait a moment.

[hoodie.store doc](http://docs.hood.ie/en/latest/api/client/hoodie.html#hoodie-store)
[hoodie.account doc](http://docs.hood.ie/en/latest/api/client/hoodie.account.html)

### tips 

We have here led strip, curl  'http://192.168.223.59/?r=775&g=1022&b=280' -X POST

* link POST requests to hoodie
* make offline-app where buttons will change colors on led strip

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
