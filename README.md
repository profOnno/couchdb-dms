# Couchdb-DMS

##Goal 
Fiddling wich couchdb and makking a simple personal Document Management System.
The idea is to store:
- Bills
- Goverment correspondance
- Hobby project schematics, drawings
- etc
- etc


##Change settings for couchdb
using couchdb with cors enabled... not secure for wan

```
curl -X PUT 127.0.0.1:5984/_config/httpd/enable_cors -d '"true"'
curl -X PUT 127.0.0.1:5984/_config/cors/origins -d '"*"'`
curl -X PUT 127.0.0.1:5984/_config/cors/credentials -d '"true"'
curl -X PUT 127.0.0.1:5984/_config/cors/credentials -d 'true'
curl -X PUT 127.0.0.1:5984/_config/cors/methods -d '"GET, PUT, POST, HEAD, DELETE"'
curl -X PUT 127.0.0.1:5984/_config/cors/headers -d '"accept, authorization, content-type, origin, referer, x-csrf-token"'
curl -X PUT 127.0.0.1:5984/_config/httpd/allow_jsonp -d '"true"'
```

