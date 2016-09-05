`browserify main.js -o bundle.js`

# Enabling Source Maps
`browserify --debug main.js -o bundle.js`

#with exorcist - create two files
- `npm install exorcist`(https://www.npmjs.com/package/exorcist)
- `browserify main.js --debug | exorcist bundle.map.js > bundle.js`

# Using Watchify
- npm install --global watchify
- `watchify main.js -o bundle.js -v`

#using beefy
- `npm install -g beefy`
- `beefy main.js --live`
- or using global browserify configuration: `beefy main.js --browserify $(which browserify) --live`

#basic browserify configuration
- Caching-Coffeify: Coffeescript support while the server is running
- Coffeeify: for Coffeescript support when we build our output bundle
- Beefy, for live reload
- Minifyify, for minfiying our bundle

-installation: `npm install --save-dev caching-coffeeify coffeeify minifyify`
