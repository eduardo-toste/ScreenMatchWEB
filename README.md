# Screenmatch Fullstack

Este repositório contém a versão fullstack do projeto **Screenmatch**, onde a aplicação foi transformada em uma API que disponibiliza os dados do banco para o frontend.

## Interface

![image](https://github.com/user-attachments/assets/4793371f-1091-497e-8826-7221d599031d)

## Tecnologias Utilizadas

### Backend
- **Java** com **Spring Boot**
- **Spring Data JPA** para persistência de dados
- **Hibernate** como ORM
- **DTOs** para transferência de dados
- **Configuração de CORS**
- **Consumo de APIs externas** (`ConsumoApi`)

### Frontend
- **HTML, CSS e JavaScript puro**
- Manipulação da DOM e requisições com `fetch()`
- Organização modular com scripts (`getDados.js`, `series.js`, `index.js`)

## Estrutura do Projeto

### Backend (server/)
```
server/
│-- src/main/java/br/com/alura/screenmatch
│   ├── config/                 # Configuração do CORS
│   ├── controller/             # Controladores REST
│   ├── dto/                    # Objetos de transferência de dados
│   ├── model/                  # Modelos de entidade do banco
│   ├── repository/             # Camada de acesso ao banco (JPA)
│   ├── service/                # Regras de negócio e consumo de APIs externas
│   ├── principal/              # Classe Principal
│-- src/main/resources/         # Configurações da aplicação
│-- application.properties      # Configurações do banco e da aplicação

```

### Frontend (client/)
```
client/
│-- css/                        # Estilos da aplicação
│-- img/                        # Imagens do projeto
│-- scripts/                     # Lógica do frontend
│   ├── getDados.js             # Requisições à API
│   ├── index.js                # Lógica da página principal
│   ├── series.js               # Manipulação de dados das séries
│-- .gitignore                  # Arquivos ignorados no versionamento
│-- detalhes.html               # Página de detalhes das séries
│-- index.html                  # Página principal
│-- styles.css                  # Estilização do site
│-- teste.js                    # Arquivo auxiliar para testes
```
