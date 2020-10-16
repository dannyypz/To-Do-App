this is a simple applications that creates a RESTful Express API. It will gives users the ablitity to CREATE, READ, UPDATE , and DELETE items from a todo list.


<!-- www.bssite.com -->

- In order to view all the todo items in this app make a http get request to /api/itmes
```

[
    {
        "id": 1,
        "item": "get some eggs",
        "completed": true
    },
    {
        "id": 2,
        "item": "get some beer",
        "completed": false
    },
]


```


- To Create a new to do list item in this app, make an http post to /api/items. the body of your post request should look like this:

```
{
    "item": "the name of the thing we're including"
}

```


- Once poster, new Item will return the following in the body of the response:


```

{
	"id": 3,
	"item": "the name of the thing we're launching",
	"completed": false
}

```


if we want to edit an item in our todo API, make a PUT requst to/api/items/:id

```
{
	"id": 2,
	"item": "get some beer",
	"completed": true
}
```


In order to delete a single item from out To do item API, make a DELETE request to /api/item/:id