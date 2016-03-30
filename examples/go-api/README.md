# Auth0 + Go API Seed
This is the seed project you need to use if you're going to create a Go Programming Language API. You'll mostly use this API either for a SPA or a Mobile app. If you just want to create a Regular Go WebApp, please check [this other seed project](https://github.com/auth0/auth0-golanglang/tree/master/examples/regular-web-app)

#Running the example
In order to run the example you need to have go and goget installed.

You also need to set the ClientSecret, ClientID and Domain for your Auth0 app as environment variables with the following names respectively: AUTH0_CLIENT_SECRET, AUTH0_CLIENT_ID and AUTH0_DOMAIN.

For that, if you just create a file named .env in the directory and set the values like the following, the app will just work:

````
# .env file
AUTH0_CLIENT_SECRET=myCoolSecret
AUTH0_CLIENT_ID=myCoolClientId
AUTH0_DOMAIN=myCoolDomain
````

Once you've set those 3 environment variables, you need to install all Go dependencies. For that, just run `go get .`.

Finally, run `go run main.go` to start the app and try calling [http://localhost:3001/ping](http://localhost:3001/ping)