# The Swagger Petstore API how-to guide

Welcome! If you're looking to familiarize yourself with the Swagger Petstore API, you've come to the right place. This how-to guide will provide a brief introduction to the Petstore API and provide a simple, step-by-step example of how to to use the API and render the response in a web page.

Let's get started!

## The Petstore API
[The Swagger Petstore API](https://petstore.swagger.io) is a RESTful API which simulates a server for a pet store. It's an excellent learning resource for fledgeling developers who are new to APIs, as it's extremely straightforward to use and requires no authorization. 

### Endpoints
The Petstore API has 3 endpoints: /pet, /store, and /user.

The **/pet** endpoint provides a number services related to, you guessed it, pets!

[View the /pet endpoint.](https://petstore.swagger.io/#/pet)

The **/store** enpoint provides services related to customer orders and store inventory.

[View the /store endpoint.](https://petstore.swagger.io/#/store)

Finally, the **/user** endpoint provides services related to users of the Petstore.

[View the /user endpoint.](https://petstore.swagger.io/#/user)

## /pet/findByStatus

For this tutorial, we will utilize the [/pet/findByStatus](https://petstore.swagger.io/#/pet/findPetsByStatus) method.

This GET call takes one parameter denoting the pet status and will return an array of all Pet objects in the database which have that status.

The API returns data in both XML and JSON. For this tutorial we'll use JSON.

The Pet object is structured thusly: 

```json
{
  "id": 0,
  "category": {
    "id": 0,
    "name": "string"
  },
  "name": "doggie",
  "photoUrls": [
    "string"
  ],
  "tags": [
    {
      "id": 0,
      "name": "string"
    }
  ],
  "status": "available"
}
```

## Test the method

You can test the method via the tool in the [method documentation](https://petstore.swagger.io/#/pet/findPetsByStatus).




## Render response in Codepen
