# Auth0 + GoLang Regular WebApp Seed
This is the seed project you need to use if you're going to create regular GoLang Webapp. If you want to create a GoLang API to use with your SPA or mobile app, please check [this other seed project](https://github.com/auth0/auth0-golang/tree/master/examples/go-api)

#Running the example
In order to run the example you need to have go and goget installed.

You also need to set the ClientSecret, ClientId, CallbackURL and Domain for your Auth0 app as environment variables with the following names respectively: `AUTH0_CLIENT_SECRET`, `AUTH0_CLIENT_ID`, `AUTH0_CALLBACK_URL` and `AUTH0_DOMAIN`.

For that, if you just create a file named `.env` in the directory and set the values like the following, the app will just work:

````bash
# .env file
AUTH0_CLIENT_SECRET=myCoolSecret
AUTH0_CLIENT_ID=myCoolClientId
AUTH0_DOMAIN=myCoolDomain
AUTH0_CALLBACK_URL=http://localhost:3000/callback
````

Once you've set those 3 environment variables, you need to install all `Go` dependencies. For that, just run `go get .`

Finally, run `go run main.go server.go` to start the app and try calling [http://localhost:3000/](http://localhost:3000/)
