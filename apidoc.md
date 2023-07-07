//page 1
> List of city
http://localhost:9120/location

> Restaurant wrt to city
http://localhost:9120/restaurants?stateId=2

>List of Quick Search
http://localhost:9120/mealType

//page 2
> Restaurant wrt to mealtype
http://localhost:9120/restaurants?mealId=2
http://localhost:9120/restaurants?stateId=1&mealId=3

> Restaurant wrt to mealtype + cuisine
http://localhost:9120/filter/1?cuisineId=2

> Restaurant wrt to mealtype + cost
http://localhost:9120/filter/1?lcost=400&hcost=1000

//page 3
> Details of Restaurant
http://localhost:9120/details/2 (details of restaurants on the basis of restaurant id)
http://localhost:9120/details/648d791b780eb24da8ebcd92 (details of restaurants on the basis of _id for that we need to import mongodb)

> Menu of Restaurant
http://localhost:9120/menu/10

//Page 4
> Details of Menu Selected 
http://localhost:9120/menuDetails
{"id":[4,8,12]}

> Place order
http://localhost:9120/placeOrder
{
    "orderId": 5,
    "name":"Priyanka",
    "email":"priyanka@gmail.com",
    "address":"Home 25",
    "phone":9999999999,
    "cost":811,
    "menuItem":[
        23,
        56,
        78
    ]
}

{
    "orderId":2,
    "name":"Amit",
    "email":"amit@gmail.com",
    "address":"Hom 65",
    "phone":"8989898989",
    "cost":612,
    "menuItem":[
        45,
        34,
        41
    ]
}

//Page 5
> List of all the orders
http://localhost:9120/orders

> Update orders details
http://localhost:9120/updateOrder
{
    "_id":"6493e7a68e9a2ee67ddfddc9",
    "status":"Out for delivery"
}

> Delete orders
http://localhost:9120/deleteOrder
{"_id:"649403c543f57ef99a5e4562"}