estoque-api (porta 8081)
Rodar o projeto: clica no ▶ verde no IntelliJ com o estoque-api aberto.
Criar banco no MySQL Workbench:
sqlUSE estoque_db;
SELECT * FROM produtos;
No Postman:
Criar produto — POST
URL: http://localhost:8081/produtos
Body (JSON):
{
    "nome": "Arroz 5kg",
    "preco": 25.90,
    "quantidade": 100,
    "descricao": "Arroz tipo 1"
}
Listar todos — GET
URL: http://localhost:8081/produtos
Buscar por ID — GET
URL: http://localhost:8081/produtos/1
Atualizar — PUT
URL: http://localhost:8081/produtos/1
Body (JSON):
{
    "nome": "Arroz 5kg",
    "preco": 27.90,
    "quantidade": 80,
    "descricao": "Arroz tipo 1 atualizado"
}
Deletar — DELETE
URL: http://localhost:8081/produtos/1
