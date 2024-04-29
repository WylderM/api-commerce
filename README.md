# E-commerce Product Management API

## Descrição

API RESTful desenvolvida para gerenciar informações de produtos em um sistema de e-commerce. Esta API permite operações CRUD em produtos, além de suportar upload de imagens para um serviço de armazenamento em nuvem.

## Tecnologias Utilizadas

- **Spring Boot** - Framework para facilitar a configuração e o desenvolvimento de novas aplicações Spring.
- **Spring Data JPA** - Para integração com bancos de dados usando JPA.
- **Spring Security** - Para autenticação e segurança das APIs.
- **AWS S3/Azure Blob Storage** - Para armazenamento de imagens dos produtos.
- **H2 Database** - Banco de dados em memória para testes locais.
- **Docker** - Para containerizar a aplicação.
- **Kubernetes** - Para orquestração dos containers.

## Configuração Inicial

### Pré-requisitos

- Java 17 ou superior
- Maven 4.0 ou superior
- Docker (opcional)
- Conta AWS/Azure para uso de S3/Blob (opcional)

### Configuração do Ambiente

Clone o repositório para sua máquina local usando:

```bash
git clone https://link-para-seu-repositorio.git
cd nome-do-repositorio
```

## Instalação das Dependências
Use o Maven para instalar todas as dependências necessárias:

```bash
mvn spring-boot:run
```
A aplicação estará disponível em http://localhost:8080.

## Dockerização
Para construir a imagem Docker da aplicação, execute:

```bash
docker build -t ecommerce-api .
```
Para rodar a aplicação usando Docker:

```bash
docker run -p 8080:8080 ecommerce-api
```

## Testando a API
Você pode usar o Postman ou qualquer outro cliente HTTP para testar as APIs. As principais rotas incluem:

- POST /produtos para adicionar um novo produto.
- GET /produtos para listar todos os produtos.
- GET /produtos/{id} para obter detalhes de um produto específico.
- PUT /produtos/{id} para atualizar um produto existente.
- DELETE /produtos/{id} para remover um produto.

## Contribuições
- Contribuições são bem-vindas. Para contribuir:

## Fork o repositório.
- Crie uma nova branch para suas modificações (git checkout -b feature/nova-feature).
- Faça suas modificações.
- Commit suas mudanças (git commit -am 'Adiciona alguma feature').
- Push para a branch (git push origin feature/nova-feature).
- Abra um Pull Request.

## Licença
Este projeto está licenciado sob a Licença MIT - veja o arquivo LICENSE.md para detalhes.

