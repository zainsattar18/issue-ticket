# PROJECT ISSUE TICKET


## Unexpected Behavior

- _On my climbs controller, when i use the create(post) method everything works except the img_url link. It return Null on postman._ 

- _Similarly, on my reviews controller, the post method gives me a 500 error. However, the put method work but only on integers and not on text. Destory works as expected._ 

## Expected Behavior

- Would like to have the methods work as expect with their respective actions rendering to postman

## Reproduce the Error

> Describe the steps we can take to reproduce the error, i.e.:

```md
1. Clone this repo.
2. Run `bundle`.
3. rails s
4. http://localhost:3000/states/1/climbs/ 
5. in postman, create new post for climbs
7. ```    {
       
        "climb_name": "Three Pines Direct",
        "img_url": "https://images.unsplash.com/photo-1527618956224-702fcb42217b?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=800&q=60",
        "type_of_climb": "Trad",
        "location": "Gunks",
        "state_id": 1
}
6. See the subsequent error in the console.
```

```

## Documentation

> Unpermitted parameter: :img_url

> - "status": 500,
    "error": "Internal Server Error",
    "exception": "#<NoMethodError: undefined method `permit' for \"new review!!\":String>",
    "traces":

```


```

## Attempted Resolution

> If you haven't already, **Google your error message now**. See if those error messages return an answer. Include at least 2 resources you've tried to consult such as walk-throughs, stack overflow articles, and other discussion threads related to your error.

```
1. (https://medium.com/better-programming/how-to-upload-images-to-a-rails-api-and-get-them-back-again-b7b3e1106a13)
2. (https://learn.co/lessons/strong-params-basics)
```