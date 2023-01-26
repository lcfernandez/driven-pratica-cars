# driven-pratica-cars

* **Prática Cars - TS + Prisma** do aluno Luiz Cláudio F. Fernandez, Turma 8 da Driven.

## Instruções para rodar localmente

* Certifique-se de ter o [Git](https://git-scm.com/), [Node](https://nodejs.org/en/) (ou [NVM](https://github.com/nvm-sh/nvm)) e [PostgreSQL](https://www.postgresql.org/download/) instalados e configurados.

* Baixe ou clone o projeto na sua máquina local.

* Certifique-se de que o servidor do PostgreSQL esteja rodando.

* Crie um banco de dados chamado `cars`.

* Crie as tabelas e popule o banco com as queries presentes no arquivo `src/config/cars.sql`.

* Na raiz do projeto, instale as dependências necessárias com o comando:

    ```
    npm i
    ```

    ou

    ```
    npm install
    ```

- Crie um arquivo `.env` preenchendo as variáveis de acordo com a configuração do banco criado anteriormente e com os devidos ajustes baseados na sua configuração local. A conexão com o banco exige uma configuração semelhante a:

    ```
    DATABASE_URL = postgres://<usuario>:<senha>@localhost:5432/<banco>?schema=public
    ```

    onde `<usuario>`, `<senha>` e `<banco>` são o usuário, senha e banco do seu ambiente local e assumindo que o Postgres esteja rodando na porta padrão (5432);

    ```
    PORT = <porta>
    ```

    onde `<porta>` é a porta desejada para que aplicação rode. Caso essa variável não seja especificada, por padrão, será feita a tentativa de conexão na porta 5000.

* Rode o projeto no ambiente de desenvolvimento com o comando:

    ```
    npm run dev
    ```

* Um servidor local estará rodando na porta 5000 (ou outra especificada no `.env`) ao ser retornada a mensagem:

    ```
    Server running on port 5000
    ```