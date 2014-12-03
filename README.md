wak-routing-pages
=================

A module to query and modify custom [views](http://doc.wakanda.org/Architecture-of-Wakanda-Applications/Page/Routing-Pages.300-1025560.en.html) in Wakanda.

Install
-------
1. Install the Modules/routing/index.js file to the solution level.
1. Edit filesystems.json at the solution level.

```
  {
  "name":"Modules",
  "parent":"SOLUTION",
  "path":"Modules",
  "writable":true
  } 
```
Example
-------
```
var modulesFolder = FileSystemSync('Modules');
var routing = require(modulesFolder.path + 'routing');

//return current array of views
routing.targets;

//add or replace a routing view (project > solution) and return updated array of views
//routing.append('Android Tablet', 'androidtab', true, '1280x800', 'Android', 'Mobile')
```

