# karoka API
A big database made with FastAPI to search everything you need in a specific location.

# Functions

# Locations
One of the main functions of the API is to provide data from a specific location.
The location will be the first thing first to know before doing any operations.

## GPS
A GPS is required to have a powerful information

## Token
A token will be generated related to the GPS location or an entered specific location if there is no activated GPS.
The token will be decrypted by karoka API to be useful. The token is needed to protect user's location.

# Models
Every model contains information and should be something specific physically or not.

## List of models

### Physical
 - Car ```RENT``` ```SELL```

### Place
 - House ```RENT``` ```SELL```
 - WC & public shower
 - University ```STUDY```
 - Hospital ```HELP```
 - Pharmacy ```MEDICAMENT SELL```

### Information
 - Exam result (BACC, BEPC, CEPE) ```FREE NEWS``` ```OFFICIAL EXAM``` 
 - Job offers ```PAID NEWS``` ```JOB```

# Endpoints
Every model has its own endpoints for CRUD operations

## List of endpoints
 - ```GET``` /<model_name> + s : returns every object of the model
 - ```GET``` /<model_name>/<model_id> : return the object with the current id
