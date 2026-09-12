### API 
---
```Application programming interface that enables communication bw different applications```


### Webfundamentals
---

## client server architeture
    ```client sends an http request to server, server process the http request and send back http response ```

### http_methods
---
`GET` => fetch all resources  
`POST` => create an new resource  
`PUT` => update a resource  
`PATCH` => UPDATE a resource (partial update)  
`DELETE` => delete a resource  


### http_request_format
---

`url`  
`http_method`  
`Authorization`  
`body`  

### sample api end point
---

```
Employee

id  name    age   department  salary

1   haris    23          hr      25000
2   vipin    23          qa      25000
3   jithn    23          it      25000
4   rahul    23          hr      25000

```

```
http_request for adding employee

url: localhost:8000/employee/
method:POST
body:{
    "name":"vysak",
    "age":24,
    "department":"hr",
    "salary":45000
}



```
---
```
http_request for listing employee

url:localhost:8000/employee/
method:GET

```

---
```
http_request for fetching specific employee detail

url : localhost:8000/employee/4/
method:GET

```

```
http_request for updating an employee 

url:localhost:8000/employee/4/
method:PUT
body:{
    "name":"Rahul",
    "age":24,
    "department":"hr",
    "salary":30000
}

```

```
http_request for deleting  specific employee 

url:localhost:8000/employee/4/
method:DELETE
```

### Movie task

```
Movie

id      title      year     language        run_time


1          kgf1      2008      kannada           160
2          kgf2      2020      kannada           165
3          kgf3      2026      kannada           167
4          kgf4      2028      kannada           168
5          kgf5      2030      kannada           169
```

`http_request for adding new movie`
url : localhost:8000/movie/
method : POST
body : {
    "title":"kgf6",
    "year":2032,
    "language":"kannada",
    "run_time":170
}


`http_request for list all movie`
url : localhost:8000/movie/
method : GET

`http_request for fetching movie detail`
url : localhost:8000/movie/3/
method : GET

`http_request for update movie`
url : localhost:8000/movie/4/
method : PUT
body : (
    "title":"leo",
    "year":2026,
    "language":"tamil",
    "run_time":160
)

`http_request for delete movie`
url : localhost:8000/movie/2/
method : DELETE

### Hospital task
```
patients

patient_id   patient_name   phone_number   assigned_doctor   department   appointment_date   status   consultation_fee
    1           aswathi      1234567890     dr jhon              ent         2026-09-06      completed       250
    2           abhi         1234567899     dr ram             ortho         2026-09-07      completed       500
    3        unnikuttan      1234567841     dr jinto       physicion         2026-09-08        pending       700
    4           viss         1234567895     dr gopal             ent         2026-09-09      completed       250
    5           yadhu        1234567555     dr vicky          dentel         2026-09-01        pending       1000

```

`http_request for adding new patients`

url : localhost:8000/patients/
method : POST
body : {
    "patient_name":"nandhu",
    "phone_number":9876543210,
    "assigned_doctor":"dr ramu",
    "department":"ent",
    "appointment_date":2026-09-10,
    "status":"completed",
    "consultation_fee":250

}

`http_request for list all patients`

url : localhost:8000/patients/
method : GET

`http_request for fetching patients detail`

url : localhost:8000/patients/2/
method : GET

`http_request for update patients`

url : localhost:8000/patients/3/
method : PUT
body : {
    "patient_name":"jithin",
    "phone_number":987654355,
    "assigned_doctor":"dr gokul",
    "department":"ortho",
    "appointment_date":2026-09-12,
    "status":"pending",
    "consultation_fee":"200"
}

`http_request for delete patients`

url : localhost:8000/patients/5/
method : DELETE

```
expenses

id  title    amount   category  owner    payment_method

1   food      230      dinner   abhi          upi
2   trip      550      water    aswathi       cash    
3   movie     700      ticket   viss          card    
4   dress     650      bill     unnikuttan    upi

```

`http_request for adding new expenses`

url : http:8000/expenses/
method : POST
body : {
    "title":"food"
    "amount":1000
    "category":"breakfast"
    "owner":"yadhu"
    "payment_method":"cash"
}

`http_request for list all expenses`

url : http:8000/expenses/
method : GET

`http_request for fetching expenses detail`

url : http:8000/expenses/4/
method : GET

`http_request for update expenses`

url : http:8000/expenses/1/
method : PUT
body : {
    "title":"car wash"
    "amount":500
    "category":"bill"
    "owner":"nandhu"
    "payment_method":"upi"    
}

`http_request for delete expenses`

url : http:8000/expenses/5/
method : DELETE