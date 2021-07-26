# LivrariaAPI

# Tecnologias utilizadas

- C#
- ASP.NET core
- Entity Framework
- SQL server
- Azure

# Sobre o projeto

  API e bancos de dados (SQL server) hospedados na Azure.
  
  Foram criados dois controllers para o teste: Authors(autores) e Publishers(editoras), podendo ser criados quantos mais se fizer necessário a partir dos models.

#Publishers

- Post:

obs: id é gerada automáticamente ao criar um publisher ou author.

  Request: https://livrariaapi2.azurewebsites.net/api/Publishers

```bash
exemplo de corpo da requisição (json):  
{
  "publisherName": "Eu Livros",
  "city": "Ourinhos",
  "state": "SP",
  "country": "BR",
  "books": [],
  "users": []
}
```

  Response:
 
```bash
{
  "pubId": <número da id>,
  "publisherName": "Eu Livros",
  "city": "Ourinhos",
  "state": "SP",
  "country": "BR",
  "books": [],
  "users": []
}
```

- GET: 

  Request: https://livrariaapi2.azurewebsites.net/api/Publishers
  
  Response:
 
```bash
[
  {
    "pubId": <número da id>,
    "publisherName": "Eu Livros",
    "city": "Ourinhos",
    "state": "SP",
    "country": "BR",
    "books": [],
    "users": []
  }
]
```
  
  Request: https://livrariaapi2.azurewebsites.net/api/Publishers/ + número da id

  Response:
 
```bash
{
  "pubId": <número da id>,
  "publisherName": "Eu Livros",
  "city": "Ourinhos",
  "state": "SP",
  "country": "BR",
  "books": [],
  "users": []
}
```


- PUT:
  
  Faz alterações em um objeto previamente criado utilizando POST.
  
  obs: id da url e do corpo da requisição devem ser, obrigatóriamente, o mesmo número.
  
  Request: https://livrariaapi2.azurewebsites.net/api/Publishers/ + número da id

```bash
exemplo de corpo da requisição (json):
{
  "pubId": <número da id>,
  "publisherName": "Você Livros",
  "city": "Ourinhos",
  "state": "SP",
  "country": "BR",
  "books": [],
  "users": []
}
```
  
  Response: No body returned for response

- DELETE:

  Request: https://livrariaapi2.azurewebsites.net/api/Publishers/ + número da id

  Response: No body returned for response

#Authors

- Post:

obs: id é gerada automáticamente ao criar um publisher ou author.

  Request: https://livrariaapi2.azurewebsites.net/api/Authors

```bash
exemplo de corpo da requisição (json):  
{
  "lastName": "Bennet",
  "firstName": "Abraham",
  "phone": "415 658-9932",
  "address": "6223 Bateman St.",
  "city": "Berkeley",
  "state": "CA",
  "zip": "94705",
  "emailAddress": "abraham.bennet@gmail.com",
  "bookAuthors": []
}
```

  Response:
 
```bash
{
  "authorId": <número da id>,
  "lastName": "Bennet",
  "firstName": "Abraham",
  "phone": "415 658-9932",
  "address": "6223 Bateman St.",
  "city": "Berkeley",
  "state": "CA",
  "zip": "94705",
  "emailAddress": "abraham.bennet@gmail.com",
  "bookAuthors": []
}
```

- GET: 

  Request: https://livrariaapi2.azurewebsites.net/api/Authors
  
  Response:
 
```bash
[
  {
    "authorId": <número da id>,
    "lastName": "Bennet",
    "firstName": "Abraham",
    "phone": "415 658-9932",
    "address": "6223 Bateman St.",
    "city": "Berkeley",
    "state": "CA",
    "zip": "94705",
    "emailAddress": "abraham.bennet@gmail.com",
    "bookAuthors": []
  }
]
```
  
  Request: https://livrariaapi2.azurewebsites.net/api/Authors/ + número da id

  Response:
 
```bash
{
  "authorId": <número da id>,
  "lastName": "Bennet",
  "firstName": "Abraham",
  "phone": "415 658-9932",
  "address": "6223 Bateman St.",
  "city": "Berkeley",
  "state": "CA",
  "zip": "94705",
  "emailAddress": "abraham.bennet@gmail.com",
  "bookAuthors": []
}
```


- PUT:
  
  Faz alterações em um objeto previamente criado utilizando POST.
  
  obs: id da url e do corpo da requisição devem ser, obrigatóriamente, o mesmo número.
  
  Request: https://livrariaapi2.azurewebsites.net/api/Authors/ + número da id

```bash
exemplo de corpo da requisição (json):
{
  "authorId": <número da id>,
  "lastName": "José",
  "firstName": "Abraham",
  "phone": "415 658-9932",
  "address": "6223 Bateman St.",
  "city": "Berkeley",
  "state": "CA",
  "zip": "94705",
  "emailAddress": "abraham.bennet@gmail.com",
  "bookAuthors": []
}
```
  
  Response: No body returned for response

- DELETE:

  Request: https://livrariaapi2.azurewebsites.net/api/Authors/ + número da id

  Response: No body returned for response

# Autor

Cauã Moreira Simião Cardoso

https://www.linkedin.com/in/cauamsimiao
