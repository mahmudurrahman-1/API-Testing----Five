# Student Report API

[![Netlify Status](https://api.netlify.com/api/v1/badges/e73ed186-e18e-48ed-ad8c-729b16ea9907/deploy-status)](https://app.netlify.com/sites/glitchmemahmud/deploys)
This API allows to reserve report of students

## [Click here to see the report](https://glitchmemahmud.netlify.app/)

## Endpoints

### Fetch All student

GET `/api/studentsDetails`

Returns the Status and data of the API.

### Status

GET `/status`

Returns the status of the API.

### Single student student in details###

GET `api/studentsDetails/169`

Returns Details of that id.
###Filter id List based in student###

GET `/api/studentsDetails?language=java`

Returns a list of students based on types.

### Create a student with student

POST `/api/studentsDetails`

Allows you to create new student details. doesn't Requires authentication.

The request body needs to be in JSON format and include the following properties:

{
"first_name": "Jawad",
"middle_name": "Ahmed",
"last_name": "Patwary",
"date_of_birth": "29/10/1995"
}

The response body returns a message
{
"id": 2675105,
"first_name": "Jawad",
"middle_name": "Ahmed",
"last_name": "Patwary",
"date_of_birth": "29/10/1995"
}

### Get newly created student

GET `/api/studentsDetails/{{id}}`

Allows you to view.

### Update a student with id

PUT `/api/studentsDetails`

Allows you to update student details. doesn't Requires authentication.

The request body needs to be in JSON format and include the following properties:
{
"id": {{Identity No}},
"first_name": "Jahid",
"middle_name": "Ahmed",
"last_name": "Patwary",
"date_of_birth": "29/10/1995"
}

The response body returns a message
{
"status": "true",
"msg": "update data success"
}

### Delete a student

Delete `/api/studentsDetails/{{id}}`

Allows you to delete students. doesn't Requires authentication.

The response body returns a message
`

- "status": "false",
- "msg": "not found"
  `
