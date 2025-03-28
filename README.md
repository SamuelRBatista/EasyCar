# EasyCar API

## Sobre o Projeto

**EasyCar API** é uma API desenvolvida com Node.js para fornecer serviços de gerenciamento de veículos. A API permite o cadastro, atualização, exclusão e consulta de veículos.

## Tecnologias Utilizadas
- Node.js
- Express.js
- TypeScript
- MySQL (banco de dados)
- Sequelize (ORM)
- JWT para autenticação
- Swagger para documentação

## Requisitos
- Node.js 18+
- Banco de dados configurado (MySQL)

## Instalação e Execução

1. Clone o repositório:
   ```sh
   git clone https://github.com/seu-usuario/EasyCarAPI.git
   cd EasyCarAPI
   ```

2. Instale as dependências do projeto:
   ```sh
   npm install
   # ou
   yarn install
   ```

3. Configure as variáveis de ambiente no arquivo `.env`:
   ```env
   PORT=3000
   DB_HOST=localhost
   DB_USER=root
   DB_PASSWORD=sua_senha
   DB_NAME=easycar
   JWT_SECRET=sua_chave_secreta
   ```

4. Execute as migrações do banco de dados:
   ```sh
   npx sequelize db:migrate
   ```

5. Inicie a API:
   ```sh
   npm run dev
   # ou
   yarn dev
   ```

6. Acesse a documentação da API (Swagger) em:
   ```
   http://localhost:3000/api-docs
   ```

## Endpoints Principais
- **GET** `/rides` - Listagem de corridas
- **POST** `/rides` - Cadastro de uma nova corrida
- **DELETE** `/rides/:ride_id` - Exclusão de uma corrida
- **GET** `/rides/:ride_id` - Detalhes de uma corrida
- **PUT** `/rides/:ride_id/finish` - Finalização de uma corrida
- **GET** `/rides/drivers/:driver_user_id` - Listagem de corridas para um motorista
- **PUT** `/rides/:ride_id/accept` - Aceitação de uma corrida
- **PUT** `/rides/:ride_id/cancel` - Cancelamento de uma corrida

## Contribuição
Contribuições são bem-vindas! Para contribuir:
1. Fork o repositório
2. Crie uma branch (`git checkout -b feature/nova-funcionalidade`)
3. Commit suas alterações (`git commit -m 'Adicionando nova funcionalidade'`)
4. Envie para o repositório remoto (`git push origin feature/nova-funcionalidade`)
5. Abra um Pull Request

## Licença
---
Desenvolvido por Samuel Ribeiro Batista

