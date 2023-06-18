# kimo-assignment

## Solution

### Models
1. there are two models chapter and courses

### API

1. `/courses` - get all the  available courses and also provided the sort functionality
      
      `name - ASCENDING , date - DESCENDING , rating - DESCENDING`


2. `/courses/{course_id}` - get the course overview for particular course

3. `/courses/{course_id}/chapters/{chapter_index}` - get specific chapter information

4. `/courses/{course_id}/chapters/{chapter_index}/rate` - this is post api to allow rate each chapter (positive / negative)


### Tests
Testing the api code. Please check in the  `tests/test_courses.py`


### Docker

`Dockerfile` also metioned for running docker container


## Run the code in local

### prerequisite 

1. python
2. pip
3. mongodb

### install dependencies

```bash
pip install -r requirements.txt
```


Change the mongodb connection string in `config.py`

### run the server

```bash
uvicorn main:app --host 0.0.0.0 --port 8000
```

### Swagger
http://localhost:8000/docs


### screenshot pdf of swagger 
![ScreenShot](https://github.com/chandankuiry/kimo-assignment/blob/main/assets/swagger.pdf)



