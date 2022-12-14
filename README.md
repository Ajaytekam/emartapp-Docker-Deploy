# emart-app

## Technology used   

* Nginx  
* Angular  
* NodeJS  
* Java  
* MongoDB  
* MySQL 

## Application Architecture 

```
                     ┌───────────────────┐
                     │Nginx (API Gateway)│
                     └───────────────────┘   
        ______________/        |        \____________
        |                      |                    |
        | "/"                  | "/api"             | "/webapi" 
        |                      |                    |
        ↓                      ↓                    ↓
┌─────────────────┐  ┌────────────────────┐  ┌─────────────────┐
│ Client(Angular) |  | NodaJS (Emart API) |  | Books API (jave)│
└─────────────────┘  └────────────────────┘  └─────────────────┘
                               |                    |      
                               ↓                    ↓
                      ┌────────────────┐      ┌──────────────┐
                      |MongoDB Database|      |Mysql Database│
                      └────────────────┘      └──────────────┘
```

## Commands to Initiate 

```
docker-compose up
```  




