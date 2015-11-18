# Sinatra Dynamic Routes Lab

## Overview
This lab will serve to reinforce your understanding of routes in a Sinatra application. Complete the following tasks in your application controller and get all of the `learn` tests to pass.

In some of the tests you might notice `%20` between words in a URL. URL's are not allowed to have spaces in them. Something like this `www.facebook.com/flatiron school` would never work as a website name. The `%` sign in a URL is called `URL encoding`. Basically, it replaces unsafe characters for a URL with appropriate ascii characters. 

You can take a look at [this list](http://www.degraeve.com/reference/urlencoding.php) for a reference on unsafe url characters, and how to use url encoding to correc them.

+ Create a dynamic route at `get '/reversename/:name'` that accepts a name and renders the name backwards.

+ Create a dynamic route at `get '/square/:number'` that accepts a number and returns the square of that number. **Note:** Remember that values in params always come in as strings, and your return value for the route should also be a string (use `.to_i` and `.to_s`).

+ Create a dynamic route at `get '/say/:number/:phrase'` that accepts a number and a phrase and returns that phrase in a string the number of times given.

+ Create a dynamic route at `get '/say/:word1/:word2/:word3/:word4/:word5'` that accepts five words and returns a string with the formatted as a sentence.

+ Create a dynamic route at `get '/:operation/:number1/:number2'` that accepts an operation (add, subtract, multiply or divide) and performs the operation on the two numbers provided. For example, going to `/add/1/2` should render `3`. 