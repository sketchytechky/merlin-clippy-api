
# Merlin's backend API

Setting up a simple express api server.

https://mobify-merlin-clippy.herokuapp.com/

## Setup

```
npm i

# run the conversion scaffold
node conversation.js

# run the dev server with hot reload
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
    'message': 'hello!',
    'context' {....}
}
```

POST reply:
```
{
    'source': 'hello!',
    'response': 'hello fellow wizard!',
    'redirectURL': 'http://www.google.com',
    'isPDP': false,
    'shouldAddToCart': true,
    // please pass this in everytime you talk to the API to make conversation sticky
    'context' {....}
}
```

### Watson magic

There's a few magic with the watson reply that we will parse

* `product description` will set isPDP true
* any embedded url in the response will set the redirectURL
* `add.*cart` will set `shouldAddToCart` true

# Watson URL

http://www.ibm.com/watson/developercloud/conversation/api/v1/?node#


# Tutorial that I copy and paste code from

Cause I'm a l33t hacker!

* https://scotch.io/tutorials/build-a-restful-api-using-node-and-express-4

* https://www.thepolyglotdeveloper.com/2015/10/create-a-simple-restful-api-with-node-js/


