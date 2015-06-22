# yeomanError
permission error solution for yeoman

## Error
   create app/styles/main.css

/usr/local/lib/node_modules/generator-angular/node_modules/yeoman-generator/node_modules/mkdirp/index.js:74
### throw err0;

###Error: EACCES, permission denied '/Users/username/Documents/Project/my-yo-angular-project/app'
    at Error (native)
    at Object.fs.mkdirSync (fs.js:747:18)
    at sync (/usr/local/lib/node_modules/generator-angular/node_modules/yeoman-generator/node_modules/mkdirp/index.js:55:12)
    at Function.sync (/usr/local/lib/node_modules/generator-angular/node_modules/yeoman-generator/node_modules/mkdirp/index.js:61:24)
    at Generator.<anonymous> (/usr/local/lib/node_modules/generator-angular/node_modules/yeoman-generator/lib/actions/actions.js:106:12)
    at processImmediate [as _immediateCallback] (timers.js:358:17)
    

## Solution
```
sudo chown username /Users/username/Documents/Project/my-yo-angular-project
