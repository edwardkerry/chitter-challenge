Chitter Challenge
=================

Overview
-------
- This is my solution to Makers Academy Week 4 challenge, producing a messaging service where people may sign up and leave short messages.
- The app is built using Ruby, on a Sinatra server. PostgreSQL is used to store user details and messages. User passwords are encrypted using BCrypt, and password retrieval e-mails are delivered via Mailgun.
- This app was test driven using RSpec for unit tests and Capybara for feature tests.


Installation instructions
-------

- Clone the repository to your local machine and change into the directory
```
$ git clone https://github.com/edwardkerry/chitter-challenge
$ cd chitter-challenge
```

- Run Bundle to acquire necessary Ruby gems `$ bundle`

- Build database and run rake migrations
```
$ createdb chitter_development
$ rake db:migrate
```

- Launch the server with Rack `$ rack`

- Visit the site `http://localhost:9292`

- Sign up and get peeping!

User Stories:
-------

```
As a Maker
So that I can post messages on Chitter as me
I want to sign up for Chitter

As a Maker
So that I can post messages on Chitter as me
I want to log in to Chitter

As a Maker
So that I can avoid others posting messages on Chitter as me
I want to log out of Chitter

As a Maker
So that I can let people know what I am doing  
I want to post a message (peep) to chitter

As a maker
So that I can see what others are saying  
I want to see all peeps in reverse chronological order

As a maker
So that I can better appreciate the context of a peep
I want to see the time at which it was made
```
