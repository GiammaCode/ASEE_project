# API NOTES 

## ENTITY CLASSES

### Film class
- titolo : string
- filmId : Int
- release : Date
- duration: Int 
- actors_inside : array Actor
- genre: String
- rating: Int

### Actor class
- actorID: Int
- name : String
- surname : String
- dateOfBirthday : Date
- filmRecite : array Film

### User class
- nome: String
- surname: String
- password: String
- email: String
- dateOfBirthday: Date
- country: String
- subscriptionPlan: String
- paymentMethod: PaymentMethod
- isActive: Boolean

### Profile class:
  - email: String
  - userName: String
  - image: String(path)
  - views : array Views 
  - raccomanded: array Raccomanded

### PaymentMethod class:
- cardType: String
- holderName: String
- cardNum: Int
- expirationDate: String
- cvv: Int

### View class:
- profile: Profile
- filmID: int
- timesOFTheFilm: Int
- isFinished: boolean

<<<<<<< HEAD
  GET{email, userName} View array
  GET{email, userName, filmID} get a View
  POST create a new view
  PUT/PATCH{email, userName, filmID}
  DELETE{email, userName,filmID}

    
  
### Recommended:
=======
### Recommended class:
>>>>>>> 444809e747dd4b33e3bc08cc618f0ef279618695
- profile: Profile
- filmID : Int
- raccomandationType: String
- Viewed: Boolean


<<<<<<< HEAD
    GET{email, userName} raccomaned array
    GET{email, userName, filmID} get a raccomanded
    POST
    PUT/PATCH{email, userName, filmID}
    DELETE{email, userName,filmID}


## API NOTES
=======
## ENDPOINTS
### Content service
- /films/
    - GET
    - POST
- /films/{id}
  - GET
  - PUT
  - PATCH
  - DELETE
- /actors
  - GET
  - POST
- /actors/{actorId}
  - GET
  - PUT
  - PATCH
- /actors/{actorId}/films
  - GET

### User service
- /users
  - GET 
  - POST
- /users/{userId}
  - GET 
  - PUT 
  - PATCH
  - DELETE
- /users/{userId}/profile
  - GET
>>>>>>> 444809e747dd4b33e3bc08cc618f0ef279618695
