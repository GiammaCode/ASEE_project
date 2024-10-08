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


### User
- nome: String
- surname: String
- password: String
- email: String
- dateOfBirthday: Date
- country: String
- subscriptionPlan: String
- paymentMethod: PaymentMethod
- isActive: Boolean



### Profile:
  - email: String
  - userName: String
  - image: String(path)
  - views : array Views 
  - raccomanded: array Raccomanded


### PaymentMethod:
- cardType: String
- holderName: String
- cardNum: Int
- expirationDate: String
- cvv: Int


### View:
- profile: Profile
- filmID: int
- timesOFTheFilm: Int
- isFinished: boolean

  GET{email, userName} View array
  GET{email, userName, filmID} get a View
  POST create a new view
  PUT/PATCH{email, userName, filmID}
  DELETE{email, userName,filmID}

    
  
### Recommended:
- profile: Profile
- filmID : Int
- raccomandationType: String
- Viewed: Boolean


    GET{email, userName} raccomaned array
    GET{email, userName, filmID} get a raccomanded
    POST
    PUT/PATCH{email, userName, filmID}
    DELETE{email, userName,filmID}


## API NOTES
