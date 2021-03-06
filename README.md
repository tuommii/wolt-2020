# Backend for Summer 2020 Internships Engineering Pre-assignment

I think [assignment](https://github.com/woltapp/summer2020) was **very fun** and well planned!

## My solution
* No external dependencies
* Endpoint accepts only POST-requests (user creates a query)
* Case-insensitive search
* Query must be legal and present, otherwise only  _message_ is returned
* For this subject, server prettifies json data
* Minimizing magic numbers
* No globals used (only constants)
* Server handles couple different HTTP Statuses
* Eslint with airbnb-base - Like
Wolt [seem's](https://github.com/woltapp/redux-autoloader/blob/master/.eslintrc) to use

## How to run it
```npm start```

Server starts listening environment variable $PORT, defined in npm scripts to be 3000.

## Test endpoint with curl
```curl -i -H "Content-Type: application/x-www-form-urlencoded" -X POST "http://localhost:3000/restaurants/search?q=City&lat=60.17045&lon=24.93147"```

```curl -i -H "Content-Type: application/x-www-form-urlencoded" -X POST "http://localhost:3000/restaurants/search?q=K%C3%A4sint&lat=60.17045&lon=24.93147"```

## How to test code
Mocha is used for testing:

```npm i```

```npm test```

