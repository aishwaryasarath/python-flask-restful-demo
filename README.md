# python-flask-restful-demo
A simple python flask RESTful demo for GET and POST

## Requirements
```
pip install flask
pip install flask-restful
```

## Run the app 
```
FLASK_APP=flask-restful.py flask run
```

## Test the endpoint for GET
```
curl http://127.0.0.1:5000/ 
```
Returns the json Hello World

<img width="228" alt="image" src="https://user-images.githubusercontent.com/49971693/158837622-ba639a9f-60d6-491c-bcbb-d8141f1d34b8.png">


## Test the /multi/num endpoint
```
curl http://127.0.0.1:5000/multi/10
```
Returns 
<img width="157" alt="image" src="https://user-images.githubusercontent.com/49971693/158837569-6d0bd3cb-6ead-4c90-9d7e-d3ad89a94e09.png">

## Test the POST endpoint with data
```
curl \
  --header "Content-Type: application/json" \
  --request POST \
  --data '{"Name":"test-name","email":"test@example.com"}' \
  http://127.0.0.1:5000/   
```

Returns {"you sent":{"Name":"test-name","email":"test@example.com"}}
