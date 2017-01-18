
# Merlin's backend API

Setting up a simple express api server.

## Setup

```
npm i

# run the conversion scaffold
node conversation.js

# run the REST server
npm run start-dev

# Test
npm run test

# Deploy
# remember to setup your heroku fella
npm run deploy
```




## API endpoint

POST /talk

POST body:
```
{
    'message': 'hello!'
}
```

POST reply:
```
{
    'source': 'hello!',
    'response': 'hello fellow wizard!',
    'redirect_url': 'http://www.google.com'
}
```


# Tutorial that I copy and paste code from

Cause I'm a l33t hacker!

* https://scotch.io/tutorials/build-a-restful-api-using-node-and-express-4

* https://www.thepolyglotdeveloper.com/2015/10/create-a-simple-restful-api-with-node-js/


