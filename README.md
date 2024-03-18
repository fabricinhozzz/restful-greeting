# RESTful Greeting
## Overview
  Esse RESTful Web Service em Spring Boot foi feito com
  base na documentação oficial do framework.
  
  Ele tem o objetivo de mandar um `Olá, Mundo!` em Spring Boot.


## Funcionality
  A aplicação provê um endpoint para recuperar uma mensagem.
  - **Endpoint:** http://localhost:8080/greeting
  - **HTTP Method:** GET
  - **Response Format:** JSON

### Response Structure
  O serviço responde com um objeto JSON, contendo as seguintes
  propriedades:
  - **id:** (Integer) Um identificador para greeting (sempre
      começando em 1).
  - **content:** (String) A saudação (como padrão, `Olá,`**name**`!`).
### Customization
  A mensagem de saudação pode ser customizada com o parâmetro opcional
  `name`, na query string: 
  - **Exemplo:** http://localhost:8080/greeting?name=fabricinhozzz


## Behavior
  - O valor no parâmetro `name` substitui o padrão (`Mundo`).
  - A resposta em objeto JSON vai refletir no nome especificado,
    na propriedade `content`.
        

