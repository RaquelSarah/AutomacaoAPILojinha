# Lojinha API Automação
Esse é um repositório que contém a automação de alguns testes de API Rest de um software denominado Lojinha.  Os sub-tópicos abaixo descrevem algumas decisões tomadas da estruturação do Projeto.

## Tecnologias Utilizadas

- Java
  https://www.oracle.com/br/java/technologies/javase/javase8u211-later-archive-downloads.html
- JUnit
  https://mvnrepository.com/artifact/org.junit.jupiter/junit-jupiter-api/5.10.0
- RestAssured
  https://mvnrepository.com/artifact/io.rest-assured/rest-assured/4.4.0
- Maven
  https://maven.apache.org/

## Testes Automatizados
Testes para validar as partições de equivalência relacionadas ao valor do produto na Lojinha, que estão vinculados diretamente à regra de negócio que diz que o valor do produto deve estar entre R$ 0,01 e R$ 7.000,00.

## Notas Gerais

- Utilizei a anotação Before Each para capturar o token que será utilizado posteriormente nos métodos de teste;
- Armazenei os dados que são enviados para API através do uso de classes POJO;
- Criei dados iniciais através de classe Data Factory, para facilitar a criação e controle dos mesmos;
- Nesse Projeto fiz uso do JUnit 5, o que me permitiu a possibilidade de usar a anotação DisplayName para dar descrições em português para os meus testes.