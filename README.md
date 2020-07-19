# Json Tranformation

## Technical stack usage:
----------------------

- Java 1.8
- Mule ESB 4
- Anypoint studio
- Maven
- Postman

## Instructions are:
---------------------

1) Import maven project into Anypoint studio
2) Right click -> Project json transformation
3) Check the console log and verify the project deployed successfully
4) Using the browsers or postman run below endpoint
5) Passing request paremeter has json value mentioned below and HTTP method must be POST
```{
   "Header":[
      "name",
      "lastName",
      "dateTime",
      "city",
      "country"
   ],
   "Items":[
      "John",
      "Smith",
      "31012019T1900Z",
      "Australia",
      "Melbourne"
   ]
}
```

## Endpoint:
-------------------
http://localhost:8081/jsontransformation


## Output Json Response:
---------------------
It will look like

```
{
  "lastname": "Smith",
  "name": "John",
  "timeZone": "",
  "offSet": "",
  "fullName": "John Smith",
  "temperatureCelcius": 0,
  "dateTime": "2020-07-19T13:13:48Z",
  "city": "Melbourne",
  "location": "Australia"
}
```
