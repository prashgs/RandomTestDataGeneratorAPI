
# Random Item Generator API


### Installation
- This API is built using FastApi(https://fastapi.tiangolo.com/) which can be installed and uvicorn server. FastApi and Uvicorn and their dependencies can be installed using below pip command both of which can be installed using  
```
pip install "fastapi[all]"
```
- Random data is generated using Faker API(https://github.com/joke2k/faker) and Mimesis(https://github.com/lk-geimfari/mimesis)
```
pip install Faker
pip install mimesis
```



### Usage
To run API server you can use ```uvicorn app:app --reload```.
Server will start at localhost and at port 8000 by default ```http://127.0.0.1:8000```
Different generators can be accessed using urls as below
```
- http://127.0.0.1:8000/addresses
- http://127.0.0.1:8000/people
```

Sample response
```
{"addresses":["301 Maldonado Walk Suite 978, North Brandon, ND 73499"]}
```

Query strings can be used to generate multiple items
```
http://127.0.0.1:8000/randomnumbers?number=5&digits=5
http://127.0.0.1:8000/people?number=5
```


FastAPI exposes API documentation through SwaggerUI and ReDoc
```
http://127.0.0.1:8000/docs
http://127.0.0.1:8000/redoc
```


### API methods
- Names Generator
- Addresses Generator
- Emailids Generator
- Company Names Generator
- Phone Numbers Generator
- Person Generator
- Texts Generator
- Random Number Generator