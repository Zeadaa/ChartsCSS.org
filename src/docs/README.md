@startuml
left to right direction

actor Buyer
actor Seller
actor Admin

rectangle "E-commerce Platform" {
    usecase "Register/Login" as UC1
    usecase "Search Products" as UC2
    usecase "Use Visual Search" as UC3
    usecase "Complete Transactions" as UC4
    usecase "Add Products" as UC5
    usecase "Manage Products" as UC6
    usecase "Monitor Activity" as UC7
    usecase "Manage Users" as UC8
}

Buyer --> UC1
Buyer --> UC2
Buyer --> UC3
Buyer --> UC4

Seller --> UC1
Seller --> UC5
Seller --> UC6

Admin --> UC1
Admin --> UC7
Admin --> UC8

@enduml
