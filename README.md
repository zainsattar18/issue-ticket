# PROJECT ISSUE TICKET


## Unexpected Behavior

-Add METHOD causing 400 error. 

## Expected Behavior

- Would like to have the request go through and add data to the page

## Reproduce the Error

> Describe the steps we can take to reproduce the error, i.e.:

- run rails server
- npm install & then npm run start
- cd into client 
- go to route "http://localhost:3001/states/2/climbs
- click add climb button and fill out form
- 



## Documentation

> 



```
Started POST "/states/2/climbs" for ::1 at 2020-07-16 15:52:39 -0400
Processing by ClimbsController#create as HTML
  Parameters: {"state_id"=>"2"}
Completed 400 Bad Request in 1ms (ActiveRecord: 0.0ms | Allocations: 116)



ActionController::ParameterMissing (param is missing or the value is empty: climb):

app/controllers/climbs_controller.rb:55:in `climb_params'
app/controllers/climbs_controller.rb:24:in `create'

```

## Attempted Resolution

> If you haven't already, **Google your error message now**. See if those error messages return an answer. Include at least 2 resources you've tried to consult such as walk-throughs, stack overflow articles, and other discussion threads related to your error.

```
https://airbrake.io/blog/http-errors/400-bad-request

```
