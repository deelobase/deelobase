
# Deelobase

![](https://www.deelobase.com/logo.png)



## Table of Contents

- [About](#about "About")
- [Features](#features "Features")
	- [Database](#database "Database")
	- [Coud Code](#cloud-code "Coud Code")
- [API](#api "API")


## About
Deelobase is a serverless NoSQL database & backend as a service that is fast, scalable, and easy to use!

## Features

### Database

- Write queries natively using JavaScript.
- Native JavaScript data types.
- Hooks.
- Can be used as a fast key-value data store.

### Cloud Code
- Write backend logic using JavaScript.
- Integrates seamlessly with Database.

## API

### Generating Keys
In order to use the API, an API key is required. To generate an API key, perform the following POST with a JSON payload:

```
curl -XPOST -H "Content-type: application/json" -d '{'email' : 'john@example.com','password':'some_password_here'}' 'https://www.deelobase.com/key/'
```
Result
```json
{
'success' : true,
'key' : 'GENERATED_API_KEY_HERE'
}
```
Note:
- email and password are required fields
- If an account does not exist, it will be created with those credentials
