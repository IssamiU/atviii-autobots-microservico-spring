# Automanager Endpoints

**Base URL:** `http://localhost:8080`

---

## Empresas
- `GET /empresa/empresas`                        - Listar todas as empresas
- `GET /empresa/{id}`                            - Buscar empresa por ID
- `POST /empresa/cadastrar`                 - Cadastrar nova empresa
- `PUT /empresa/atualizar/{id}`                  - Atualizar empresa existente
- `DELETE /empresa/excluir/{id}`                 - Excluir empresa
- `POST /empresa/{empresaId}/usuario/{usuarioId}`- Associar usuário à empresa
- `DELETE /empresa/{empresaId}/usuario/{usuarioId}` - Remover usuário da empresa
- `GET /empresa/{empresaId}/usuarios`            - Listar usuários da empresa

---

## Usuários
- `GET /usuario/usuarios`         - Listar todos os usuários
- `GET /usuario/{id}`             - Buscar usuário por ID
- `POST /usuario/cadastrar`       - Cadastrar novo usuário
- `PUT /usuario/atualizar`        - Atualizar usuário existente
- `DELETE /usuario/excluir`       - Excluir usuário

---

## Mercadorias
- `GET /mercadoria/mercadorias`   - Listar todas as mercadorias
- `GET /mercadoria/{id}`          - Buscar mercadoria por ID
- `POST /mercadoria/cadastro`     - Cadastrar nova mercadoria
- `PUT /mercadoria/atualizar`     - Atualizar mercadoria existente
- `DELETE /mercadoria/excluir`    - Excluir mercadoria

---

## Serviços
- `GET /servico/servicos`         - Listar todos os serviços
- `GET /servico/{id}`             - Buscar serviço por ID
- `POST /servico/cadastro`        - Cadastrar novo serviço
- `PUT /servico/atualizar`        - Atualizar serviço existente
- `DELETE /servico/excluir`       - Excluir serviço

---

## Veículos
- `GET /veiculo/veiculos`         - Listar todos os veículos
- `GET /veiculo/{id}`             - Buscar veículo por ID
- `POST /veiculo/cadastrar`       - Cadastrar novo veículo
- `PUT /veiculo/atualizar`        - Atualizar veículo existente
- `DELETE /veiculo/excluir`       - Excluir veículo

---

## Vendas
- `GET /venda/vendas`             - Listar todas as vendas
- `GET /venda/{id}`               - Buscar venda por ID
- `POST /venda/cadastro`          - Cadastrar nova venda
- `PUT /venda/atualizar`          - Atualizar venda existente
- `DELETE /venda/excluir`         - Excluir venda

---

## Credenciais
- `GET /credencial/credenciais`   - Listar todas as credenciais
- `GET /credencial/{id}`          - Buscar credencial por ID