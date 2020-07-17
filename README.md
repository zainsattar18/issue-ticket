# PROJECT ISSUE TICKET


## Unexpected Behavior

-Post Method for Reviews controller is giving me 422 

## Expected Behavior

- Would like to have the request go through and add data to the page

## Reproduce the Error

> Describe the steps we can take to reproduce the error, i.e.:

- run rails server
- npm install & then npm run start
- cd into client 
- go to to reviews and add new review
- add data to clim
- 



## Documentation

> 



```
rocessing by ReviewsController#create as HTML
  Parameters: {"review"=>{"review"=>"fgbbgfbg", "rating"=>"2", "img_url"=>"https://images.unsplash.com/photo-1502126324834-38f8e02d7160?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=800&q=60"}, "climb_id"=>"1"}
  User Load (1.0ms)  SELECT "users".* FROM "users" WHERE "users"."id" = $1 LIMIT $2  [["id", 3], ["LIMIT", 1]]
  ↳ app/controllers/application_controller.rb:19:in `authorize_request'
   (0.3ms)  BEGIN
  ↳ app/controllers/reviews_controller.rb:37:in `create'
  Climb Load (0.3ms)  SELECT "climbs".* FROM "climbs" WHERE "climbs"."id" = $1 LIMIT $2  [["id", 1], ["LIMIT", 1]]
  ↳ app/controllers/reviews_controller.rb:37:in `create'
   (0.2ms)  ROLLBACK
  ↳ app/controllers/reviews_controller.rb:37:in `create'
Completed 422 Unprocessable Entity in 41ms (Views: 0.2ms | ActiveRecord: 1.8ms | Allocations: 4022)

```

## Attempted Resolution

> If you haven't already, **Google your error message now**. See if those error messages return an answer. Include at least 2 resources you've tried to consult such as walk-throughs, stack overflow articles, and other discussion threads related to your error.

```
http://weblog.jamisbuck.org/2007/2/5/nesting-resources
https://www.youtube.com/watch?v=T0lcUENA8zs
```
