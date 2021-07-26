# LivrariaAPI

# Sobre o projeto

API com código escalável feita com banco de dados SQL server e hospedada na Azure.

# Tecnologias utilizadas

- C#
- ASP.NET core
- Entity Framework
- SQL server
- Azure

# Como executar o projeto

Programa utilizado para teste: insomnia.
obs: pode-se usar outros semelhantes, como o postman.
obs': foram criados dois controllers para o teste: Authors(autores) e Publishers(editoras), podendo ser criados quantos mais necessários a partir dos models.

Após aberto o insomnia ou semelhante, criar as requisições: GET, POST, PUT e DELETE.

Requisições:


- POST, utilizar url: https://livrariaapi2.azurewebsites.net/api/Authors ou https://livrariaapi2.azurewebsites.net/api/Publishers.

obs: id é gerada automáticamente ao criar um publisher ou author.

```bash
exemplo de corpo da requisição (json): 
Authors:
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
  
Publishers:
{
  "publisherName": "Eu Livros",
  "city": "Ourinhos",
  "state": "SP",
  "country": "BR",
  "books": [],
  "users": []
}
```

- GET: 

Para mostrar todos, utilizar url: https://livrariaapi2.azurewebsites.net/api/Authors ou https://livrariaapi2.azurewebsites.net/api/Publishers.

Para mostrar apenas um, utilizar url: https://livrariaapi2.azurewebsites.net/api/Authors/ + número da id ou https://livrariaapi2.azurewebsites.net/api/Publishers/ + número da id


- PUT, utilizar url: https://livrariaapi2.azurewebsites.net/api/Authors/ + número da id ou https://livrariaapi2.azurewebsites.net/api/Publishers/ + número da id

obs: id da url e do corpo da requisição devem ser, obrigatóriamente, o mesmo número.

Faz alterações em um objeto previamente criado utilizando POST.

```bash
exemplo de corpo da requisição (json):
Authors:
{
  "authorId": 1,
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

Publishers:
 {
  "pubId": 1,
  "publisherName": "Você Livros",
  "city": "Ourinhos",
  "state": "SP",
  "country": "BR",
  "books": [],
  "users": []
}
```

- DELETE, utilizar url: https://livrariaapi2.azurewebsites.net/api/Authors/ + número da id ou https://livrariaapi2.azurewebsites.net/api/Publishers/ + número da id

obs: será excluído o objeto da id informada na url.

# Autor

Cauã Moreira Simião Cardoso

https://www.linkedin.com/in/cauamsimiao
