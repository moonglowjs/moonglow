# moonglow
Framework for simple business with mongoose and mongodb

I want to make a higher database access framework for mongodb with mongoose;
```js
let whatyouwant = moonglow.bussiness.operation(filter,option)

// with [host, database_name[, port] signature
var db = mongoose.createConnection('localhost', 'database', port)
```

### the interfaces for user is like this:

```js
const moonglow = require('moonglow');

//dbSpec can be uid|token|whatever that can specifice the database connection for the business.
let dbSpec = uid;
let userInfo = moonglow.user.getById(uid, dbSpec);
let users = moonglow.user.getById([uid],dbSpec);

let empls = moonglow.group.find({},dbSpec);


let opts = {page:{skip, limit}};
let todos = moonglow.todo.find({uid}, opts,dbSpec);

```
