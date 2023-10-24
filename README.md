<h1 align="center">
  Epic Task
</h1>

<p align="center">
 <img src="https://img.shields.io/static/v1?label=Type&message=Project&color=red&labelColor=000000" alt="Project" />
</p>

API para gerenciar tarefas (CRUD) para o o gerenciamento de tarefas.


## Tecnologias
 
- [Spring Data JPA](https://spring.io/projects/spring-data-jpa)
- [Spring Thymeleaf](https://docs.spring.io/spring-framework/reference/web/webmvc-view/mvc-thymeleaf.html)
- [Spring Validation](https://spring.io/guides/gs/validating-form-input/)
- [Spring Web](https://spring.io/guides/gs/spring-boot/)
- [Spring Oauth2 Client](https://spring.io/guides/tutorials/spring-boot-oauth2/)
- [Spring DevTools](https://docs.spring.io/spring-boot/docs/2.1.5.RELEASE/reference/html/using-boot-devtools.html)
- [Spring H2](https://www.baeldung.com/spring-boot-h2-database)
- [Spring Lombok](https://www.baeldung.com/intro-to-project-lombok)
- [Spring MVC](https://docs.spring.io/spring-framework/reference/web/webmvc.html)

## Práticas adotadas

- SOLID, DRY, YAGNI, KISS
- API REST
- Consultas com Spring Data JPA
- Injeção de Dependências
- Tratamento de respostas de erro

## Como Executar

- Clonar repositório git
- Construir o projeto:
```
$ ./mvnw clean package
```
- Executar a aplicação:
```
$ java -jar target/epictasklist-0.0.1-SNAPSHOT.jar
```

A API poderá ser acessada em [localhost:8080](http://localhost:8080).
O Swagger poderá ser visualizado em [localhost:8080/swagger-ui.html](http://localhost:8080/swagger-ui.html)

## API Endpoints

Para fazer as requisições HTTP abaixo, foi utilizada a ferramenta [httpie](https://httpie.io):

- Criar Tarefa 
```
$ http POST :8080/todos nome="YYY" XXX="YYY" XXX=YYY

[
  {
    "XXX": "YYY",
    "XXX": YYY,
    "XXX": "YYY",
    "XXX": YYY,
    "XXX": YYY
  }
]
```

- Listar XXX
```
$ http GET :8080/XXX

[
  {
    "XXX": "YYY",
    "XXX": YYY,
    "XXX": "YYY",
    "XXX": YYY,
    "XXX": YYY
  }
]
```

- Atualizar XXX
```
$ http PUT :8080/XXX/YYY XXX="YYY" XXX="YYY" XXX=YYY

[
  {
   "XXX": "YYY",
    "XXX": YYY,
    "XXX": "YYY",
    "XXX": YYY,
    "XXX": YYY
  }
]
```

- Remover XXX
```
http DELETE :8080/XXX/YYY

[ ]
```
