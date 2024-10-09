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
- paymentMethod: String
- isActive: Boolean

### Profile class:
  - email: String
  - userName: String
  - image: String(path)
  - views : array Views 
  - raccomanded: array Raccomanded


### View:
- profile: Profile
- filmID: int
- timesOFTheFilm: Int
- isFinished: boolean


### Recommended:
- profile: Profile
- filmID : Int
- raccomandationType: String
- Viewed: Boolean




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
  - DELETE
- /users/{userId}/profile
  - GET
  - POST
- - /users/{userId}/profile/profile{id}
  - GET
  - PUT
  - DELETE



### Raccomandation Service

- /users/{userId}/profiles/{profileId}/views
  - GET 
  - POST
  
- /users/{userId}/profiles/{profileId}/views/{filmID}
  -  GET
  - PUT
  - DELETE
  

  
- /users/{userId}/profiles/{profileId}/raccomanded
  - GET
  - POST

- /users/{userId}/profiles/{profileId}/raccomanded/{filmID}
  - GET
  - PUT
  - DELETE

# API NOTES