## Note if running locally use 'npm run local' to start the backend.
## EndPoints

## Resume EndPoints (Roman)
**Add Resume**

Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

POST: https://smartresumebuild.herokuapp.com/api/resume/add

Request:
```javascript
{
  "user_id": "5f2661a29ee13a46dc8edf4f",
  "title": "FullStack Dev Resume",
  "description": "Resume sent to Shopify for FullStack Developer Position"
}
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2b9e08d133e500171a210f",
        "user_id": "5f2661a29ee13a46dc8edf4f",
        "title": "FullStack Dev Resume",
        "description": "Resume sent to Shopify for FullStack Developer Position",
        "__v": 0
    }
}
```
**Get Resume By Id**

Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

GET: https://smartresumebuild.herokuapp.com/api/resume/5f2b9c7fd133e500171a210e

Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2b9e08d133e500171a210f",
        "user_id": "5f2661a29ee13a46dc8edf4f",
        "title": "FullStack Dev Resume",
        "description": "Resume sent to Shopify for FullStack Developer Position",
        "__v": 0
    }
}
```

**Get Resume List By UserId**

Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

GET: https://smartresumebuild.herokuapp.com/api/resume/list/5f2661a29ee13a46dc8edf4f

Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": [
        {
            "_id": "5f2b9e08d133e500171a210f",
            "user_id": "5f2661a29ee13a46dc8edf4f",
            "title": "FullStack Dev Resume",
            "description": "Resume sent to Shopify for FullStack Developer Position",
            "__v": 0
        },
       ............
    ]
}
```

**Delete Resume**

Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

DELETE: https://smartresumebuild.herokuapp.com/api/resume

Request:
```javascript
{
    "id": "5f2b9c7fd133e500171a210e"
}
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2b9eb7d133e500171a2110",
        "user_id": "5f2661a29ee13a46dc8edf4f",
        "title": "FullStack Dev Resume",
        "description": "Resume sent to Shopify for FullStack Developer Position",
        "__v": 0
    }
}
```


**Update Resume**

Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

PUT: https://smartresumebuild.herokuapp.com/api/resume

Request:
```javascript
{
  "id": "5f2b9e08d133e500171a210f",
  "user_id": "5f2661a29ee13a46dc8edf4f",
  "title": "Mobile Engineer Position",
  "description": "Resume for Amazon Mobile Dev"  
}
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2b9e08d133e500171a210f",
        "user_id": "5f2661a29ee13a46dc8edf4f",
        "title": "Mobile Engineer Position",
        "description": "Resume for Amazon Mobile Dev",
        "__v": 0
    }
}
```

## Job Profile EndPoints (Roman)
**Add Job Profile**

Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

POST: https://smartresumebuild.herokuapp.com/api/jobprofile/add

Request:
```javascript
{
  "user_id": "5f2661a29ee13a46dc8edf4f",
  "profile": "10 years of experience in every software ever created"
}
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2b9c4ad133e500171a210d",
        "user_id": "5f2661a29ee13a46dc8edf4f",
        "profile": "10 years of experience in every software ever created",
        "__v": 0
    }
}
```
**Get Job Profile By Id**

Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

GET: https://smartresumebuild.herokuapp.com/api/jobprofile/5f2b9c7fd133e500171a210e

Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2b9c7fd133e500171a210e",
        "user_id": "5f2661a29ee13a46dc8edf4f",
        "profile": "An expert at cross functional synergy",
        "__v": 0
    }
}
```

**Get Job Profile List By UserId**

Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

GET: https://smartresumebuild.herokuapp.com/api/jobprofile/list/5f2661a29ee13a46dc8edf4f

Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": [
        {
            "_id": "5f2b9c4ad133e500171a210d",
            "user_id": "5f2661a29ee13a46dc8edf4f",
            "profile": "10 years of experience in every software ever created",
            "__v": 0
        },
        ..........
    ]
}
```

**Delete Job Profile**

Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

DELETE: https://smartresumebuild.herokuapp.com/api/jobprofile

Request:
```javascript
{
    "id": "5f2b9c7fd133e500171a210e"
}
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2b9c7fd133e500171a210e",
        "user_id": "5f2661a29ee13a46dc8edf4f",
        "profile": "An expert at cross functional synergy",
        "__v": 0
    }
}
```


**Update Job Profile**

Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

PUT: https://smartresumebuild.herokuapp.com/api/jobprofile

Request:
```javascript
{
   "id": "5f2b9c4ad133e500171a210d",
  "user_id": "5f2661a29ee13a46dc8edf4f",
  "profile": "Clearly the best man for the job"
  
  }
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2b9c4ad133e500171a210d",
        "user_id": "5f2661a29ee13a46dc8edf4f",
        "profile": "Clearly the best man for the job",
        "__v": 0
    }
}
```


## Objective EndPoints (Roman)
**Add Objective**

Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

POST: https://smartresumebuild.herokuapp.com/api/objective/add

Request:
```javascript
{
  "user_id": "5f2661a29ee13a46dc8edf4f",
  "objective": "To put a roof over my head"
}
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2b9569d133e500171a210b",
        "user_id": "5f2661a29ee13a46dc8edf4f",
        "objective": "To put a roof over my head",
        "__v": 0
    }
}
```
**Get Objective By Id**

Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

GET: https://smartresumebuild.herokuapp.com/api/objective/5f2b9569d133e500171a210b

Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2b9569d133e500171a210b",
        "user_id": "5f2661a29ee13a46dc8edf4f",
        "objective": "To put a roof over my head",
        "__v": 0
    }
}
```

**Get Objective List By UserId**

Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

GET: https://smartresumebuild.herokuapp.com/api/objective/list/5f2661a29ee13a46dc8edf4f

Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": [
        {
            "_id": "5f2b9569d133e500171a210b",
            "user_id": "5f2661a29ee13a46dc8edf4f",
            "objective": "To put a roof over my head",
            "__v": 0
        }
		.....
    ]
}
```

**Delete Objective**

Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

DELETE: https://smartresumebuild.herokuapp.com/api/objective

Request:
```javascript
{
    "id": "5f2b9698d133e500171a210c"
}
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2b9698d133e500171a210c",
        "user_id": "5f2661a29ee13a46dc8edf4f",
        "objective": "Make more money than ever",
        "__v": 0
    }
}
```


**Update Objective**

Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

PUT: https://smartresumebuild.herokuapp.com/api/objective

Request:
```javascript
{
   "id": "5f2b9569d133e500171a210b",
  "user_id": "5f2661a29ee13a46dc8edf4f",
  "objective": "To make the worls a better place."  
}
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2b9569d133e500171a210b",
        "user_id": "5f2661a29ee13a46dc8edf4f",
        "objective": "To make the worls a better place.",
        "__v": 0
    }
}
```

## Education EndPoints (Roman)
**Add Education**

Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

POST: https://smartresumebuild.herokuapp.com/api/education/add

Request:
```javascript
{
  "user_id": "5f29e49520781d0017b465b9",
  "school": "University of Toronto",
  "degree": "Masters",
  "field": "Computer Science",
  "start": "2000",
  "finish": "2010"
}
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2b008a899f8100176e3da9",
        "user_id": "5f29e49520781d0017b465b9",
        "school": "University of Toronto",
        "degree": "Masters",
        "field": "Computer Science",
        "start": "2000",
        "finish": "2010",
        "__v": 0
    }
}
```
**Get Education By Id**

Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

GET: https://smartresumebuild.herokuapp.com/api/education/5f29e5ee20781d0017b465ba

Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f29e5ee20781d0017b465ba",
        "user_id": "5f29e49520781d0017b465b9",
        "school": "Humber College",
        "degree": "Masters",
        "field": "IT",
        "start": "2000",
        "finish": "2010",
        "__v": 0
    }
}
```

**Get Education List By UserId**

Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

GET: https://smartresumebuild.herokuapp.com/api/education/list/5f29e49520781d0017b465b9

Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": [
        {
            "_id": "5f29e5ee20781d0017b465ba",
            "user_id": "5f29e49520781d0017b465b9",
            "school": "Humber College",
            "degree": "Masters",
            "field": "IT",
            "start": "2000",
            "finish": "2010",
            "__v": 0
        },
        {
            "_id": "5f2b008a899f8100176e3da9",
            "user_id": "5f29e49520781d0017b465b9",
            "school": "University of Toronto",
            "degree": "Masters",
            "field": "Computer Science",
            "start": "2000",
            "finish": "2010",
            "__v": 0
        }
    ]
}
```

**Delete Education**

Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

DELETE: https://smartresumebuild.herokuapp.com/api/education

Request:
```javascript
{
    "id": "5f29e5ee20781d0017b465ba"
}
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f29e5ee20781d0017b465ba",
        "user_id": "5f29e49520781d0017b465b9",
        "school": "Humber College",
        "degree": "Masters",
        "field": "IT",
        "start": "2000",
        "finish": "2010",
        "__v": 0
    }
}
```


**Update Education**

Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

PUT: https://smartresumebuild.herokuapp.com/api/education

Request:
```javascript
{
   "id": "5f2b041753e6352e9403850f",
  "user_id": "5f2b03ba53e6352e9403850e",
  "school": "University of Cape Town",
  "degree": "Masters",
  "field": "IT",
  "start": "2000",
  "finish": "2005"
}
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2b041753e6352e9403850f",
        "user_id": "5f2b03ba53e6352e9403850e",
        "school": "University of Cape Town",
        "degree": "Masters",
        "field": "IT",
        "start": "2000",
        "finish": "2005",
        "__v": 0
    }
}
```

## Authentication EndPoints (Hung)
**User Registration**

POST: https://smartresumebuild.herokuapp.com/api/auth/register

Request:
```javascript
{
    "email": "nguyenvuluan89@gmail.com",
    "password": "12345",
    "confirmedPassword": "12345"
}
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2b72ef54af050017dd4223",
        "created_date": "2020-08-06T03:03:11.526Z",
        "email": "nguyenvuluan89@gmail.com",
        "__v": 0
    }
}
```

**User Login**

POST: https://smartresumebuild.herokuapp.com/api/auth/login

Request:
```javascript
{
    "email": "nguyenvuluan89@gmail.com",
    "password": "12345"
}
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "email": "nguyenvuluan89@gmail.com",
        "accessToken": "{token}"
    }
}
```

## Skill EndPoints (Hung)
**Add Skill**
Authorization Header Required:
Authorization: Bearer UserAuthTokenHere
POST: https://smartresumebuild.herokuapp.com/api/skill/add

Request:
```javascript
{
    "user_id": "5f2b72ef54af050017dd4223",
    "skill_name": "HTML",
    "is_hard_skill": false
}
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2be447f2864e0017f9f482",
        "user_id": "5f2b72ef54af050017dd4223",
        "skill_name": "HTML",
        "is_hard_skill": false,
        "__v": 0
    }
}
```

**Get Skill List By UserId**
Authorization Header Required:
Authorization: Bearer UserAuthTokenHere
GET: https://smartresumebuild.herokuapp.com/api/skill/list/{user-id}

Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": [
        {
            "_id": "5f2be447f2864e0017f9f482",
            "user_id": "5f2b72ef54af050017dd4223",
            "skill_name": "HTML",
            "is_hard_skill": false,
            "__v": 0
        }
    ]
}
```

**Delete Skill**
Authorization Header Required:
Authorization: Bearer UserAuthTokenHere
DELETE: https://smartresumebuild.herokuapp.com/api/skill

Request:
```javascript
{
    "id": "{skill_id}"
}
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2be447f2864e0017f9f482",
        "user_id": "5f2b72ef54af050017dd4223",
        "skill_name": "HTML",
        "is_hard_skill": false,
        "__v": 0
    }
}
```

**Update Skill**
Authorization Header Required:
Authorization: Bearer UserAuthTokenHere
PUT: https://smartresumebuild.herokuapp.com/api/skill

Request:
```javascript
{
    "id": "5f2be5e8f2864e0017f9f483",
    "user_id": "5f2b72ef54af050017dd4223",
    "skill_name": "CSS",
    "is_hard_skill": false
}
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2be5e8f2864e0017f9f483",
        "user_id": "5f2b72ef54af050017dd4223",
        "skill_name": "CSS",
        "is_hard_skill": false,
        "__v": 0
    }
}
```

## Project EndPoints (Hung)
**Add Project**
Authorization Header Required:
Authorization: Bearer UserAuthTokenHere
POST: https://smartresumebuild.herokuapp.com/api/project/add

Request:
```javascript
{
    "user_id": "5f2b72ef54af050017dd4223",
    "name": "ABC",
    "description": ".NET developer"
}
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2be8e79a74fa71399dc24f",
        "user_id": "5f2b72ef54af050017dd4223",
        "name": "ABC",
        "description": ".NET developer",
        "__v": 0
    }
}
```
**Get Project By Id**
Authorization Header Required:
Authorization: Bearer UserAuthTokenHere
GET: https://smartresumebuild.herokuapp.com/api/project/{project-id}

Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "duties": [],
        "skills": [],
        "_id": "5f2be8e79a74fa71399dc24f",
        "user_id": "5f2b72ef54af050017dd4223",
        "name": "ABC",
        "description": ".NET developer",
        "__v": 0
    }
}
```

**Get Porject List By UserId**
Authorization Header Required:
Authorization: Bearer UserAuthTokenHere
GET: https://smartresumebuild.herokuapp.com/api/project/list/{user-id}

Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": [
        {
            "duties": [],
            "skills": [],
            "_id": "5f2be8e79a74fa71399dc24f",
            "user_id": "5f2b72ef54af050017dd4223",
            "name": "ABC",
            "description": ".NET developer",
            "__v": 0
        }
    ]
}
```

**Delete Project**
Authorization Header Required:
Authorization: Bearer UserAuthTokenHere
DELETE: https://smartresumebuild.herokuapp.com/api/project

Request:
```javascript
{
    "id": "{project_id}"
}
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "duties": [],
        "skills": [],
        "_id": "5f2be8e79a74fa71399dc24f",
        "user_id": "5f2b72ef54af050017dd4223",
        "name": "ABC",
        "description": "Senior .NET developer",
        "__v": 0
    }
}
```

**Update Project**
Authorization Header Required:
Authorization: Bearer UserAuthTokenHere
PUT: https://smartresumebuild.herokuapp.com/api/project

Request:
```javascript
{
    "id": "5f2be8e79a74fa71399dc24f",
    "user_id": "5f2b72ef54af050017dd4223",
    "name": "ABC",
    "description": "Senior .NET developer"
}
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2be8e79a74fa71399dc24f",
        "user_id": "5f2b72ef54af050017dd4223",
        "name": "ABC",
        "description": "Senior .NET developer",
        "__v": 0
    }
}
```


## Language EndPoints (Luan)
**Add Language**
Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

POST: https://smartresumebuild.herokuapp.com/api/language/add

Request:
```javascript
{
    "user_id": "5f2b72ef54af050017dd4223",
    "language": "English",
    "proficiency": "Professional working proficiency"
}
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2b73c154af050017dd4224",
        "created_date": "2020-08-06T03:06:41.992Z",
        "user_id": "5f2b72ef54af050017dd4223",
        "language": "English",
        "proficiency": "Professional working proficiency",
        "__v": 0
    }
}
```
**Get Language By Id**
Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

GET: https://smartresumebuild.herokuapp.com/api/language/{language-id}

Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2b73c154af050017dd4224",
        "created_date": "2020-08-06T03:06:41.992Z",
        "user_id": "5f2b72ef54af050017dd4223",
        "language": "English",
        "proficiency": "Professional working proficiency",
        "__v": 0
    }
}
```

**Get Language List By UserId**
Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

GET: https://smartresumebuild.herokuapp.com/api/language/list/{user-id}

Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": [
        {
            "_id": "5f2b73c154af050017dd4224",
            "created_date": "2020-08-06T03:06:41.992Z",
            "user_id": "5f2b72ef54af050017dd4223",
            "language": "English",
            "proficiency": "Professional working proficiency",
            "__v": 0
        }
    ]
}
```

**Delete Language**
Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

DELETE: https://smartresumebuild.herokuapp.com/api/language

Request:
```javascript
{
    "id": "{language_id}"
}
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2b73c154af050017dd4224",
        "created_date": "2020-08-06T03:06:41.992Z",
        "user_id": "5f2b72ef54af050017dd4223",
        "language": "English",
        "proficiency": "Professional working proficiency",
        "__v": 0
    }
}
```

**Update Language**
Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

PUT: https://smartresumebuild.herokuapp.com/api/language

Request:
```javascript
{
    "id": "5f0a8d1fa380783ef49936d8",
    "user_id": "5f0a819684a234361cf9421c",
    "language": "Vietnamese2",
    "proficiency": "Professional working proficiency"
}
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2b755b54af050017dd4225",
        "created_date": "2020-08-06T03:13:31.365Z",
        "user_id": "5f2b72ef54af050017dd4223",
        "language": "Vietnamese 2",
        "proficiency": "Professional working proficiency",
        "__v": 0
    }
}
```

## Experience EndPoints (Luan)
**Add Experience**
Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

POST: https://smartresumebuild.herokuapp.com/api/experience/add

Request:
```javascript
{
    "user_id": "5f2b72ef54af050017dd4223",
    "title": "Front-end developer",
    "type": "Part-time",
    "company": "IGNITE",
    "location": "Toronto",
    "start_date": "08/15/2019",
    "end_date": "08/15/2020",
    "description": "test"
}
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2b897fcaf53c0017ead0b7",
        "start_date": "2019-08-15T00:00:00.000Z",
        "end_date": "2020-08-15T00:00:00.000Z",
        "user_id": "5f2b72ef54af050017dd4223",
        "title": "Front-end developer",
        "type": "Part-time",
        "company": "IGNITE",
        "location": "Toronto",
        "description": "test",
        "__v": 0
    }
}
```
**Get Experience By Id**
Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

GET: https://smartresumebuild.herokuapp.com/api/experience/{experience-id}

Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2b85b4a1276e67f5156bbe",
        "start_date": "2019-08-06T00:00:00.000Z",
        "end_date": "2020-08-06T00:00:00.000Z",
        "user_id": "5f0a819684a234361cf9421c",
        "title": "Front-end developer",
        "type": "Part-time",
        "company": "IGNITE",
        "location": "Toronto",
        "description": "test",
        "__v": 0
    }
}
```

**Get Experience List By UserId**
Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

GET: https://smartresumebuild.herokuapp.com/api/experience/list/{user-id}

Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": [
        {
            "_id": "5f2b897fcaf53c0017ead0b7",
            "start_date": "2019-08-15T00:00:00.000Z",
            "end_date": "2020-08-15T00:00:00.000Z",
            "user_id": "5f2b72ef54af050017dd4223",
            "title": "Front-end developer",
            "type": "Part-time",
            "company": "IGNITE",
            "location": "Toronto",
            "description": "test",
            "__v": 0
        }
    ]
}
```

**Delete Language**
Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

DELETE: https://smartresumebuild.herokuapp.com/api/experience

Request:
```javascript
{
    "id": "{experience-id}"
}
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2b897fcaf53c0017ead0b7",
        "start_date": "2019-08-15T00:00:00.000Z",
        "end_date": "2020-08-15T00:00:00.000Z",
        "user_id": "5f2b72ef54af050017dd4223",
        "title": "Front-end developer",
        "type": "Part-time",
        "company": "IGNITE",
        "location": "Toronto",
        "description": "test",
        "__v": 0
    }
}
```

**Update Experience**
Authorization Header Required:

Authorization: Bearer UserAuthTokenHere

PUT: https://smartresumebuild.herokuapp.com/api/experience

Request:
```javascript
{
    "id": "5f2b8b60caf53c0017ead0b8",
    "user_id": "5f2b72ef54af050017dd4223",
    "title": "Front-end developer 2",
    "type": "Part-time",
    "company": "IGNITE",
    "location": "Toronto",
    "start_date": "08/15/2019",
    "end_date": "08/15/2020",
    "description": "test"
}
```
Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": {
        "_id": "5f2b8b60caf53c0017ead0b8",
        "start_date": "2019-08-15T00:00:00.000Z",
        "end_date": "2020-08-15T00:00:00.000Z",
        "user_id": "5f2b72ef54af050017dd4223",
        "title": "Front-end developer 2",
        "type": "Part-time",
        "company": "IGNITE",
        "location": "Toronto",
        "description": "test",
        "__v": 0
    }
}
```

## CoverLetter EndPoints (Michael)
**Add CoverLetter**

Authorization Header Required:

Authorization: Bearer UserAuthToken Here

POST: https://smartresumebuild.herokuapp.com/api/coverletter/add

Request:
```javascript
        {
            "user_id": "5f278d28cf154530147bcf95",
            "title": "React JS Developer",
            "body": "Working hard to do more"
        }
```
**Get CoverLetter By Id**

Authorization Header Required:

Authorization: Bearer UserAuthToken Here

GET: https://smartresumebuild.herokuapp.com/api/coverletter/5f279580cf154530147bcf97

Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data":{
	"_id":"5f279580cf154530147bcf97",
	"created_date":"2020-08-03T04:41:36.094+00:00",
	"user_id":"5f278d28cf154530147bcf95",
	"title":"Java Developer",
	"body":"I'm the best I'm the best I'm the best fit for your Java dev team",
	"__v":{"$numberInt":"0"}}
}
```

**Get CoverLetter List By UserId**

Authorization Header Required:

Authorization: Bearer UserAuthToken Here

GET: https://smartresumebuild.herokuapp.com/api/coverletter/list/5f278d28cf154530147bcf95

Response:
```javascript
{
    "isSuccess": true,
    "message": "",
    "data": [        
	{	"_id":"5f279580cf154530147bcf97",
	"created_date":"2020-08-03T04:41:36.094+00:00",
	"user_id":"5f278d28cf154530147bcf95",
	"title":"Java Developer",
	"body":"I'm the best I'm the best I'm the best fit for your Java dev team",
	"__v":{"$numberInt":"0"}
	},	
	{
	"_id":"5f27966fcf154530147bcf98",
	"created_date":"2020-08-03T04:45:35.481+00:00",
	"user_id":"5f278d28cf154530147bcf95",
	"title":"FullStack Developer",
	"body":" I'm the best for your backend stuff",
	"__v":{"$numberInt":"0"}
	},
	{
	"_id":"5f2b28536bfd18097898e156",
	"created_date":"2020-08-05T21:44:51.984+00:00",
	"user_id":"5f278d28cf154530147bcf95",
	"title":"React JS Developer",
	"body":"Working hard to do more",
	"__v":{"$numberInt":"0"}}
    ]
}
```

**Delete CoverLetter**

Authorization Header Required:

Authorization: Bearer UserAuthToken Here

DELETE: https://smartresumebuild.herokuapp.com/api/coverletter

Request:
```javascript
{
    "id": "5f279580cf154530147bcf97"
}
```


**Update CoverLetter**

Authorization Header Required:

Authorization: Bearer UserAuthToken Here

PUT: https://smartresumebuild.herokuapp.com/api/coverletter

Request:
```javascript
       {
            "id": "5f2b28536bfd18097898e156",
            "user_id": "5f278d28cf154530147bcf95",
            "title": "React JS Developer",
            "body": "Working hard to do better"
        }
```
## BasicInfo EndPoints (Michael)
**Add BasicInfo**

Authorization Header Required:

Authorization: Bearer UserAuthToken Here

POST: https://smartresumebuild.herokuapp.com/api/basicinfo/add

Request:
```javascript
        {
    "user_id": "5f278d28cf154530147bcf95",
    "firstName": "Michael",
    "lastName": "Anetor",
    "email": "michellanet@gmail.com",
    "phone": "6120808080",
    "address": "1 Main St E",
    "country": "Canada",
    "region": "Ontario",
    "gitHub": "https://github.com/devBoy",
    "linkedin": "https://www.linkedin.com/in/michael-anetor"
}
```
**Get BasicInfo By Id**

Authorization Header Required:

Authorization: Bearer UserAuthToken Here

GET: https://smartresumebuild.herokuapp.com/api/basicinfo/5f2b28cc6bfd18097898e157

Response:
```javascript
{
            "_id": "5f2b28cc6bfd18097898e157",
            "created_date": "2020-08-05T21:46:52.650Z",
            "user_id": "5f278d28cf154530147bcf95",
            "firstName": "Michael",
            "lastName": "Anetor",
            "email": "michellanet@gmail.com",
            "phone": "6120808080",
            "address": "1 Main St E",
            "country": "Canada",
            "region": "Ontario",
            "gitHub": "https://github.com/devBoy",
            "linkedin": "https://www.linkedin.com/in/michael-anetor",
            "__v": 0
        }
```

**Get BasicInfo List By UserId**

Authorization Header Required:

Authorization: Bearer UserAuthToken Here

GET: https://smartresumebuild.herokuapp.com/api/basicinfo/list/5f278d28cf154530147bcf95

Response:
```javascript
{
            "_id": "5f2b28cc6bfd18097898e157",
            "created_date": "2020-08-05T21:46:52.650Z",
            "user_id": "5f278d28cf154530147bcf95",
            "firstName": "Michael",
            "lastName": "Anetor",
            "email": "michellanet@gmail.com",
            "phone": "6120808080",
            "address": "1 Main St E",
            "country": "Canada",
            "region": "Ontario",
            "gitHub": "https://github.com/devBoy",
            "linkedin": "https://www.linkedin.com/in/michael-anetor",
            "__v": 0
        }
```

**Delete BasicInfo**

Authorization Header Required:

Authorization: Bearer UserAuthToken Here

DELETE: https://smartresumebuild.herokuapp.com/api/basicinfo

Request:
```javascript
{
    "id": "5f2b28cc6bfd18097898e157"
}
```


**Update BasicInfo**

Authorization Header Required:

Authorization: Bearer UserAuthToken Here

PUT: https://smartresumebuild.herokuapp.com/api/basicinfo

Request:
```javascript
       {
            "id": "5f2b28cc6bfd18097898e157",
            "created_date": "2020-08-05T21:46:52.650Z",
            "user_id": "5f278d28cf154530147bcf95",
            "firstName": "Michael",
            "lastName": "Anetor",
            "email": "michellanet@gmail.com",
            "phone": "6120808080",
            "address": "1 Main St E",
            "country": "Canada",
            "region": "Ontario",
            "gitHub": "https://github.com/devBoy",
            "linkedin": "https://www.linkedin.com/in/michael-anetor",
            "__v": 0
        }
```

# Front-End

Front-End uses React

## Setup

Go to the frontend folder /frontend, then create .env from .env.example

## Installation

Install the packages

```bash
npm install
```

## Usage

```python
npm start
```

# Back-End

Back-End uses Express and MongoDB

## Setup

Go to the frontend folder /backend, then create .env from .env.example

## Installation

Install the packages

```bash
npm install
```

## Usage

```python
npm run local
```


