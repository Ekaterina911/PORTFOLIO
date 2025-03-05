## Swagger
# GET /api​/v1​/Activities
1. HTTP-метод:GET 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Activities  
3. Заголовки запроса:-H  "accept: text/plain; v=1.0" 
4. Тело запроса (при наличии): отсутствует  
5. Статус-код ответа: 200  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
 ```
 {
    "id": 1,
    "title": "Activity 1",
    "dueDate": "2023-06-14T12:03:55.2578262+00:00",
    "completed": false
  },
```

 # POST /api​/v1​/Activities
1. HTTP-метод:POST  
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Activities 
3. Заголовки запроса:-H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0" -d "{\"id\":0,\"title\":\"string\",\"dueDate\":\"2023-06-14T11:20:56.818Z\",\"completed\":true}"  
4. Тело запроса (при наличии):  
```
 {
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-14T11:20:56.818Z",
  "completed": true
} 
```  
5. Статус-код ответа: 200   
6. Тело ответа (при наличии). Если тело большое, то только его часть: 

 ```
 {
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-14T11:20:56.818Z",
  "completed": true
}  
```
# GET /api/v1/Activities/{3}
1. HTTP-метод:GET 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Activities/3
3. Заголовки запроса:-H  "accept: text/plain; v=1.0"
4. Тело запроса (при наличии): отсутствует  
5. Статус-код ответа: 200  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
 ```
 {
  "id": 3,
  "title": "Activity 3",
  "dueDate": "2023-06-14T14:32:53.2298567+00:00",
  "completed": false
}
```
# GET /api/v1/Activities/{377777777777}
1. HTTP-метод:GET 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Activities/377777777777
3. Заголовки запроса:-H  "accept: text/plain; v=1.0"
4. Тело запроса (при наличии): отсутствует  
5. Статус-код ответа: 400  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
 ```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-7b0c5c0b876b6b41a94f5c630d4ee8d7-c2d3400ba4312e4e-00",
  "errors": {
    "id": [
      "The value '377777777777' is not valid."
    ]
  }
}
```
# GET /api/v1/Activities/{37}
1. HTTP-метод:GET 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Activities/37
3. Заголовки запроса:-H  "accept: text/plain; v=1.0"
4. Тело запроса (при наличии): отсутствует  
5. Статус-код ответа: 404  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
 ```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-5e523f2193f5064e8842caf2c75c216f-09ece0909282e740-00"
}
```
# PUT /api/v1/Activities/{3}
1. HTTP-метод:PUT 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Activities/3  
3. Заголовки запроса:-H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0" -d "{\"id\":0,\"title\":\"string\",\"dueDate\":\"2023-06-14T12:06:15.582Z\",\"completed\":true}"  
4. Тело запроса (при наличии):
```
 {
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-14T12:06:15.582Z",
  "completed": true
}  
```

5. Статус-код ответа: 200  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
```
{
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-14T12:06:15.582Z",
  "completed": true
}
```
# PUT /api/v1/Activities/{3890998459999}
1. HTTP-метод:PUT 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Activities/3890998459999
3. Заголовки запроса:-H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0" -d "{\"id\":0,\"title\":\"string\",\"dueDate\":\"2023-06-14T12:06:15.582Z\",\"completed\":true}" 
4. Тело запроса (при наличии):
```
 {
  "id": 0,
  "title": "string",
  "dueDate": "2023-06-14T12:06:15.582Z",
  "completed": true
} 
```

5. Статус-код ответа: 400  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-fadc6647e49f1a4383e7de5326c8446a-78f2d1e39e992643-00",
  "errors": {
    "id": [
      "The value '3890998459999' is not valid."
    ]
  }
}
```
# DELETE /api/v1/Activities/{3}
1. HTTP-метод:DELETE 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Activities/3 
3. Заголовки запроса:-H  "accept: */*"  
4. Тело запроса (при наличии):отсутствует
5. Статус-код ответа: 200  
6. Тело ответа (при наличии). Если тело большое, то только его часть:отсутствует

# DELETE /api/v1/Activities/{356789098765432}
1. HTTP-метод:DELETE 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Activities/356789098765432
3. Заголовки запроса:-H  "accept: */*"  
4. Тело запроса (при наличии):отсутствует
5. Статус-код ответа: 400  
6. Тело ответа (при наличии). Если тело большое, то только его часть:
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-b9ff60fe7c29954dbadc6939409f0b97-dc97284564974a4f-00",
  "errors": {
    "id": [
      "The value '356789098765432' is not valid."
    ]
  }
}
```
# GET /api/v1/Authors
1. HTTP-метод:GET 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Authors
3. Заголовки запроса: -H  "accept: text/plain; v=1.0"
4. Тело запроса (при наличии): отсутствует  
5. Статус-код ответа: 200  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
 ```
 {
    "id": 1,
    "idBook": 1,
    "firstName": "First Name 1",
    "lastName": "Last Name 1"
  },
  {
    "id": 2,
    "idBook": 1,
    "firstName": "First Name 2",
    "lastName": "Last Name 2"
  },
```
# POST /api/v1/Authors
1. HTTP-метод:POST 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Authors
3. Заголовки запроса: -H  "accept: text/plain; v=1.0"
4. Тело запроса (при наличии): 
 ```
{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}  
 ```
5. Статус-код ответа: 200  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
 ```
 {
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
# GET /api/v1/Authors/authors/books/{12}
1. HTTP-метод:GET 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/12
3. Заголовки запроса: -H  "accept: text/plain; v=1.0"
4. Тело запроса (при наличии): отсутствует  
5. Статус-код ответа: 200  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
 ```
{
    "id": 35,
    "idBook": 12,
    "firstName": "First Name 35",
    "lastName": "Last Name 35"
  },
  {
    "id": 36,
    "idBook": 12,
    "firstName": "First Name 36",
    "lastName": "Last Name 36"
```
# GET /api/v1/Authors/authors/books/{1265789098765}
1. HTTP-метод:GET 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Authors/authors/books/1265789098765
3. Заголовки запроса: -H  "accept: text/plain; v=1.0"
4. Тело запроса (при наличии): отсутствует  
5. Статус-код ответа: 400  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
 ```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-21382fb4bba73b4abc966f0b36bad057-4fcf8fd5ec4b5442-00",
  "errors": {
    "idBook": [
      "The value '1265789098765' is not valid."
    ]
  }
}
```
# GET /api/v1/Authors/{88}
1. HTTP-метод:GET 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Authors/88
3. Заголовки запроса: -H  "accept: text/plain; v=1.0"
4. Тело запроса (при наличии): отсутствует  
5. Статус-код ответа: 200  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
 ```
{
  "id": 88,
  "idBook": 30,
  "firstName": "First Name 88",
  "lastName": "Last Name 88"
}
```
# GET /api/v1/Authors/{8866666666}
1. HTTP-метод:GET 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Authors/8866666666
3. Заголовки запроса: -H  "accept: text/plain; v=1.0"
4. Тело запроса (при наличии): отсутствует  
5. Статус-код ответа: 400  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
 ```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-4904c679d0beaa46a641a497c3cf7290-d30c863a9c11b44a-00",
  "errors": {
    "id": [
      "The value '8866666666' is not valid."
    ]
  }
}
```
# PUT /api/v1/Authors/{8}
1. HTTP-метод:PUT 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Authors/8 
3. Заголовки запроса:-H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0" -d "{\"id\":0,\"idBook\":0,\"firstName\":\"string\",\"lastName\":\"string\"}"  
4. Тело запроса (при наличии):
```
{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}  
```

5. Статус-код ответа: 200  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
```
{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
# PUT /api/v1/Authors/{32323232323}
1. HTTP-метод:PUT 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Authors/32323232323
3. Заголовки запроса:-H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0" -d "{\"id\":0,\"title\":\"string\",\"dueDate\":\"2023-06-14T12:06:15.582Z\",\"completed\":true}" 
4. Тело запроса (при наличии):
```
{
  "id": 0,
  "idBook": 0,
  "firstName": "string",
  "lastName": "string"
}
```
5. Статус-код ответа: 400  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-0cf32e490c2c684f9f2322db15b5b06b-205bce11f5a6ed45-00",
  "errors": {
    "id": [
      "The value '32323232323' is not valid."
    ]
  }
}
```
# DELETE /api/v1/Authors/{33}
1. HTTP-метод:DELETE 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Authors/33
3. Заголовки запроса:-H  "accept: */*"  
4. Тело запроса (при наличии):отсутствует
5. Статус-код ответа: 200  
6. Тело ответа (при наличии). Если тело большое, то только его часть:отсутствует

# DELETE /api/v1/Authors/{3333333333}
1. HTTP-метод:DELETE 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Authors/3333333333
3. Заголовки запроса:-H  "accept: */*"  
4. Тело запроса (при наличии):отсутствует
5. Статус-код ответа: 400  
6. Тело ответа (при наличии). Если тело большое, то только его часть:
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-498d98862b56be48b59ee2de9fd66293-3c7cafae311e0b43-00",
  "errors": {
    "id": [
      "The value '3333333333' is not valid."
    ]
  }
}
```
# GET /api/v1/Books
1. HTTP-метод:GET 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Books  
3. Заголовки запроса:-H  "accept: text/plain; v=1.0" 
4. Тело запроса (при наличии): отсутствует  
5. Статус-код ответа: 200  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
 ```
 {
    "id": 1,
    "title": "Book 1",
    "description": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "pageCount": 100,
    "excerpt": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
    "publishDate": "2023-06-13T20:20:27.1768638+00:00"
  },
```
# POST /api/v1/Books
1. HTTP-метод:POST  
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Books
3. Заголовки запроса:-H  "accept: */*" -H  "Content-Type: application/json; v=1.0" -d "{\"id\":0,\"title\":\"string\",\"description\":\"string\",\"pageCount\":0,\"excerpt\":\"string\",\"publishDate\":\"2023-06-14T20:22:38.723Z\"}"  
4. Тело запроса (при наличии):  
```
{
  "id": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-14T20:22:38.723Z"
} 
```  
5. Статус-код ответа: 200   
6. Тело ответа (при наличии). Если тело большое, то только его часть: 

 ```
{
  "id": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-14T20:22:38.723Z"
} 
```
# GET /api/v1/Books/{17}
1. HTTP-метод:GET 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Books/17 
3. Заголовки запроса:-H  "accept: text/plain; v=1.0"
4. Тело запроса (при наличии): отсутствует  
5. Статус-код ответа: 200  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
 ```
{
  "id": 17,
  "title": "Book 17",
  "description": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
  "pageCount": 1700,
  "excerpt": "Lorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\nLorem lorem lorem. Lorem lorem lorem. Lorem lorem lorem.\n",
  "publishDate": "2023-05-28T20:24:49.0065391+00:00"
}
```
# GET /api/v1/Books/{177789876543}
1. HTTP-метод:GET 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Books/177789876543
3. Заголовки запроса:-H  "accept: text/plain; v=1.0"
4. Тело запроса (при наличии): отсутствует  
5. Статус-код ответа: 400  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
 ```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-13a8a417405a8e48a3deaaa32a963dd0-7b0945c221af0f44-00",
  "errors": {
    "id": [
      "The value '177789876543' is not valid."
    ]
  }
}
```
# PUT /api/v1/Books/{10}
1. HTTP-метод:PUT 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Books/10
3. Заголовки запроса:-H  "accept: */*" -H  "Content-Type: application/json; v=1.0" -d "{\"id\":0,\"title\":\"string\",\"description\":\"string\",\"pageCount\":0,\"excerpt\":\"string\",\"publishDate\":\"2023-06-14T20:28:14.180Z\"}" 
4. Тело запроса (при наличии):
```
{
  "id": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-14T20:28:14.180Z"
}
```

5. Статус-код ответа: 200  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
```
{
  "id": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-14T20:28:14.18Z"
}
```
# PUT /api/v1/Books/{10101010101}
1. HTTP-метод:PUT 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Books/10101010101
3. Заголовки запроса:-H  "accept: -H  "accept: */*" -H  "Content-Type: application/json; v=1.0" -d "{\"id\":0,\"title\":\"string\",\"description\":\"string\",\"pageCount\":0,\"excerpt\":\"string\",\"publishDate\":\"2023-06-14T20:28:14.180Z\"}"
4. Тело запроса (при наличии):
```
{
  "id": 0,
  "title": "string",
  "description": "string",
  "pageCount": 0,
  "excerpt": "string",
  "publishDate": "2023-06-14T20:28:14.180Z"
}
```
5. Статус-код ответа: 400  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-c8ba112da4ef0c42a8a83433b41e5fab-8fac1b7b7d43a446-00",
  "errors": {
    "id": [
      "The value '10101010101' is not valid."
    ]
  }
}
```
# DELETE /api/v1/Books/{90}
1. HTTP-метод:DELETE 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Books/90
3. Заголовки запроса:-H  "accept: */*"  
4. Тело запроса (при наличии):отсутствует
5. Статус-код ответа: 200  
6. Тело ответа (при наличии). Если тело большое, то только его часть:отсутствует

# DELETE /api/v1/Authors/{9000000000}
1. HTTP-метод:DELETE 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Books/9000000000
3. Заголовки запроса:-H  "accept: */*"  
4. Тело запроса (при наличии):отсутствует
5. Статус-код ответа: 400  
6. Тело ответа (при наличии). Если тело большое, то только его часть:
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-4aa341aa1090a148a0e87c1434360a10-7dd2e93bbe8a5d4b-00",
  "errors": {
    "id": [
      "The value '9000000000' is not valid."
    ]
  }
}
```
# GET /api/v1/CoverPhotos
1. HTTP-метод:GET 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos 
3. Заголовки запроса:-H  "accept: text/plain; v=1.0" 
4. Тело запроса (при наличии): отсутствует  
5. Статус-код ответа: 200  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
 ```
{
    "id": 1,
    "idBook": 1,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 1&w=250&h=350"
  },
  {
    "id": 2,
    "idBook": 2,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 2&w=250&h=350"
  },
```
# POST /api/v1/CoverPhotos
1. HTTP-метод:POST  
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos
3. Заголовки запроса:-H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0" -d "{\"id\":0,\"idBook\":0,\"url\":\"string\"}" 
4. Тело запроса (при наличии):  
```
{
  "id": 0,
  "idBook": 0,
  "url": "string"
} 
```  
5. Статус-код ответа: 200   
6. Тело ответа (при наличии). Если тело большое, то только его часть: 

 ```
{
  "id": 0,
  "idBook": 0,
  "url": "string"
}
```
# GET /api/v1/CoverPhotos/books/covers/{34}
1. HTTP-метод:GET 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/34
3. Заголовки запроса:-H  "accept: text/plain; v=1.0" 
4. Тело запроса (при наличии): отсутствует  
5. Статус-код ответа: 200  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
 ```
[
  {
    "id": 34,
    "idBook": 34,
    "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 34&w=250&h=350"
  }
]
```
# GET /api/v1/CoverPhotos/books/covers/{3444444444}
1. HTTP-метод:GET 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/books/covers/3444444444
3. Заголовки запроса:-H  "accept: text/plain; v=1.0" 
4. Тело запроса (при наличии): отсутствует  
5. Статус-код ответа: 400  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
 ```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-d228be232df2ee4ea881ae08bd994159-a57198aa297d874e-00",
  "errors": {
    "idBook": [
      "The value '3444444444' is not valid."
    ]
  }
}
```
# GET /api/v1/CoverPhotos/{29}
1. HTTP-метод:GET 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/29
3. Заголовки запроса:-H  "accept: text/plain; v=1.0" 
4. Тело запроса (при наличии): отсутствует  
5. Статус-код ответа: 200  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
 ```
{
  "id": 29,
  "idBook": 29,
  "url": "https://placeholdit.imgix.net/~text?txtsize=33&txt=Book 29&w=250&h=350"
}
```
# GET /api/v1/CoverPhotos/{345}
1. HTTP-метод:GET 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/345
3. Заголовки запроса:-H  "accept: text/plain; v=1.0" 
4. Тело запроса (при наличии): отсутствует  
5. Статус-код ответа: 404  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
 ```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-7a1afe7a3442404ea063c9d0581d2961-b87dc81f0f6d8649-00"
}
```

# PUT /api/v1/CoverPhotos/{123}
1. HTTP-метод:PUT 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/123
3. Заголовки запроса:-H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0" -d "{\"id\":0,\"idBook\":0,\"url\":\"string\"}"
4. Тело запроса (при наличии):
```
{
  "id": 0,
  "idBook": 0,
  "url": "string"
}
```
5. Статус-код ответа: 200  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
```
{
  "id": 0,
  "idBook": 0,
  "url": "string"
}
```
# PUT /api/v1/CoverPhotos/{12345678910}
1. HTTP-метод:PUT 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/12345678910
3. Заголовки запроса:-H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0" -d "{\"id\":0,\"idBook\":0,\"url\":\"string\"}"
4. Тело запроса (при наличии):
```
{
  "id": 0,
  "idBook": 0,
  "url": "string"
}
```
5. Статус-код ответа: 400  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-38e7b4961dbfd94fb48d599eea7e618b-baaf3d4dbd43a947-00",
  "errors": {
    "id": [
      "The value '12345678910' is not valid."
    ]
  }
}
```
# DELETE /api/v1/CoverPhotos/{33}
1. HTTP-метод:DELETE 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/CoverPhotos/33
3. Заголовки запроса:-H  "accept: */*"  
4. Тело запроса (при наличии):отсутствует
5. Статус-код ответа: 200  
6. Тело ответа (при наличии). Если тело большое, то только его часть:отсутствует

# DELETE /api/v1/CoverPhotos/{3344444444}
1. HTTP-метод:DELETE 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Authors/3344444444
3. Заголовки запроса:-H  "accept: */*"  
4. Тело запроса (при наличии):отсутствует
5. Статус-код ответа: 400  
6. Тело ответа (при наличии). Если тело большое, то только его часть:
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-19e6b6680c76ea46b4a82a3005e65123-582e7f6c50108645-00",
  "errors": {
    "id": [
      "The value '3344444444' is not valid."
    ]
  }
}
```
# GET /api/v1/Users
1. HTTP-метод:GET 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Users 
3. Заголовки запроса:-H  "accept: text/plain; v=1.0" 
4. Тело запроса (при наличии): отсутствует  
5. Статус-код ответа: 200  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
 ```
{
    "id": 1,
    "userName": "User 1",
    "password": "Password1"
  },
  {
    "id": 2,
    "userName": "User 2",
    "password": "Password2"
  },
```
# POST /api/v1/Users
1. HTTP-метод:POST  
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Users
3. Заголовки запроса:-H  "accept: */*" -H  "Content-Type: application/json; v=1.0" -d "{\"id\":0,\"userName\":\"string\",\"password\":\"string\"}"
4. Тело запроса (при наличии):  
```
{
  "id": 0,
  "userName": "string",
  "password": "string"
}

```  
5. Статус-код ответа: 200   
6. Тело ответа (при наличии). Если тело большое, то только его часть: 

 ```
{
  "id": 0,
  "userName": "string",
  "password": "string"
}
```
# GET /api/v1/Users/{2}
1. HTTP-метод:GET 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Users/2
3. Заголовки запроса:-H  "accept: */*" 
4. Тело запроса (при наличии): отсутствует  
5. Статус-код ответа: 200  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
 ```
{
  "id": 2,
  "userName": "User 2",
  "password": "Password2"
}
```
# GET /api/v1/Users/{11}
1. HTTP-метод:GET 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Users/11
3. Заголовки запроса:-H  "accept: */*" 
4. Тело запроса (при наличии): отсутствует  
5. Статус-код ответа: 404  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
 ```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.4",
  "title": "Not Found",
  "status": 404,
  "traceId": "00-77e4ee1aa7c1bd449aaa7a7f44845e07-3a1a657390c1c340-00"
}
```
# PUT /api/v1/Users/{11}
1. HTTP-метод:PUT 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Users/11
3. Заголовки запроса:--H  "accept: */*" -H  "Content-Type: application/json; v=1.0" -d "{\"id\":0,\"userName\":\"string\",\"password\":\"string\"}"
4. Тело запроса (при наличии):
```
{
  "id": 0,
  "userName": "string",
  "password": "string"
}
```
5. Статус-код ответа: 200  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
```
{
  "id": 0,
  "userName": "string",
  "password": "string"
}
```
# PUT /api/v1/Users/{11111111111}
1. HTTP-метод:PUT 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Users/11111111111
3. Заголовки запроса:-H  "accept: text/plain; v=1.0" -H  "Content-Type: application/json; v=1.0" -d "{\"id\":0,\"idBook\":0,\"url\":\"string\"}"
4. Тело запроса (при наличии):
```
{
  "id": 0,
  "userName": "string",
  "password": "string"
}
```
5. Статус-код ответа: 400  
6. Тело ответа (при наличии). Если тело большое, то только его часть:  
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-4d1c1fe2b7f2a84194f917337ec041d4-7f72e2fe859eb445-00",
  "errors": {
    "id": [
      "The value '11111111111' is not valid."
    ]
  }
}
```
# DELETE /api/v1/Users/{45}
1. HTTP-метод:DELETE 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Users/45
3. Заголовки запроса:-H  "accept: */*"  
4. Тело запроса (при наличии):отсутствует
5. Статус-код ответа: 200  
6. Тело ответа (при наличии). Если тело большое, то только его часть:отсутствует

# DELETE /api/v1/Users/{4550000003}
1. HTTP-метод:DELETE 
2. Полный URL запроса:https://fakerestapi.azurewebsites.net/api/v1/Users/4550000003
3. Заголовки запроса:-H  "accept: */*"  
4. Тело запроса (при наличии):отсутствует
5. Статус-код ответа: 400  
6. Тело ответа (при наличии). Если тело большое, то только его часть:
```
{
  "type": "https://tools.ietf.org/html/rfc7231#section-6.5.1",
  "title": "One or more validation errors occurred.",
  "status": 400,
  "traceId": "00-bc4ccc4ab083904885a11112ea65d0c1-f8d4e7110bb4ff48-00",
  "errors": {
    "id": [
      "The value '4550000003' is not valid."
    ]
  }
}
```
