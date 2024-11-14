# API REST de Produtos com Spring Boot

API RESTful para gerenciar uma lista de produtos, com operações CRUD e tratamento de erros para produtos inexistentes.

## Endpoints

| Método | Endpoint           | Função                             |
|--------|---------------------|------------------------------------|
| `GET`  | `/produtos`        | Retorna todos os produtos         |
| `POST` | `/produtos`        | Cria um novo produto              |
| `GET`  | `/produtos/{id}`   | Busca produto por ID              |
| `PUT`  | `/produtos/{id}`   | Atualiza um produto por ID        |
| `DELETE` | `/produtos/{id}` | Remove um produto por ID          |

## Estrutura do Projeto

### Entidade Produto

- `ID` (Long)
- `Nome` (String)
- `Descrição` (String)
- `Preço` (Decimal)
- `Quantidade em Estoque` (Integer)

### Exemplo de Respostas

- **GET /produtos**: Retorna uma lista de produtos
- **GET /produtos/{id}**: Retorna um produto específico ou mensagem "Produto não encontrado"
- **POST /produtos**: Cria um produto novo com os dados fornecidos
- **PUT /produtos/{id}**: Atualiza os detalhes de um produto existente
- **DELETE /produtos/{id}**: Remove um produto ou informa que o produto não foi encontrado

## Como Executar

1. Clone o repositório e execute o projeto:
   ```bash
   ./mvnw spring-boot:run
2. A API utiliza um banco de dados em memória H2. Para acessar o console H2, vá para http://localhost:8080/h2-console.
3. Execute testes unitários com JUnit e Mockito para validação de funcionalidades.

