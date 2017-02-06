# Rails as an API Study

Use your favorite search engine and the provided readings to research and
respond to the following questions.

In your responses, be sure to cite any relevant sources you consulted in your
search. We ask you to write responses in your own words in order to see how you
process what you've read. Please do not respond with direct quotes from source
material. Instead, digest what you've read and repeat it in your own voice.

Please note:

-   Many of the readings will mention the "view" layer. We won't be covering the
    view layer in this program.
-   We'll use our [Rails API Template](https://github.com/ga-wdi-boston/rails-api-template)
    repository as the basis for our rails applications.
    This template excludes the "view" layer.

## Required Readings

-   Better Explained
    -   [Starting Ruby on Rails: What I Wish I Knew](http://betterexplained.com/articles/starting-ruby-on-rails-what-i-wish-i-knew/)
        (sections 3 and 4)
    -   [Intermediate Rails: Understanding Models, Views and Controllers](http://betterexplained.com/articles/intermediate-rails-understanding-models-views-and-controllers/)
        (up to and including "Quick Controllers")
-   Ruby on Rails Guides
    -   [Rails Routing from the Outside](http://guides.rubyonrails.org/routing.html)
        (up to and including chapter 2.6)
    -   [Action Controller Overview](http://guides.rubyonrails.org/action_controller_overview.html)
        (up to and including chapter 4.5)
    -   [The Rails Command Line](http://guides.rubyonrails.org/command_line.html)
        (up to and including chapter 1.4)

## Additional Resources

-   [Getting Started with Rails — Ruby on Rails Guides](http://guides.rubyonrails.org/getting_started.html)

## Define Model Responsiblities

In your own words, define what the responsibilities of the model layer are in
Rails.

```md
The Model layer in Rails is responsible for accessing the data requested by the user.  It takes the request from the controller and talks to the database.  It does whatever action it is told to do by the controller on the database, then sends the response back to the controller as a string.
```

## Define Controller Responsiblities

In your own words, define what the responsibilities of the controller layer are
in Rails.

```md
The Controller layer in Rails is responsible for talking to the router and taking the request given by the user.  It takes the request and tells the appropriate model what data to access and what action to perform on it.  It sends the response it gets back to the client.
```

## Define Router Responsiblities

In your own words, define what the router does in Rails.

```md
The Router in Rails takes the client's requests on resources and routes them to the proper controller.  It essentially organizes the requests for the controller so that the controller can continue the request as fast as possible.
```

## The Request-Response Cycle in Rails

Starting with a client making a GET request to a particular URL, describe how
the parts of Rails interact to produce and send a response.

```md
First, a client makes a GET request.  This request is sent to the server and is first picked up by the router.  The router organizes the request or requests and sends them to the appropriate controller.  The controller then tells the appropriate models what data to access and what actions to perform on it.  The Model then accesses the databases and performs the appropriate actions as dictated by the controller.  It then sends a response string to the controller, which sends the response to the client.  
```
