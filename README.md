couchbase-co
============

couchbase-co for node-couchbase

<h2>Usage</h2>

node --harmony
>co = require('co');
>couchbaseClient = require('./index.js');
>couchbase = new couchbaseClient(['xxxx:11311'], 'user', 'passwd');
>co(function *(){
> yield couchbase.Set('key', 'val', null, timestamp)
> yield couchbase.Get('key');
> yield couchbase.Del('key');
>})();
