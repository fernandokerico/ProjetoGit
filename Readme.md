# PLANO DE TESTES
#### Nome do Projeto: Teste de Funcionalidades para o Marketplace ServeRest.

**Resumo do Planejamento:** Este plano de testes visa garantir que as funcionalidades CRUD para os recursos de autenticação, produtos e usuários no Marketplace ServeRest estejam funcionando conforme o esperado.

**Pessoas Envolvidas:**
* Cliente/Usuário.
* Desenvolvedor.
* Analista de teste.

**Funcionalidade:** Funcionalidades CRUD para autenticação, produtos e usuários.

**Recursos Necessários:**
* Software: Ferramentas de teste (como Postman, Sweggear, GitHub e Jira).
* Rede: Acesso à rede local para acessar as ferramentas.
* Word para documentar o plano de testes, levantar cenários e as rotas.

**Critérios Usados:**
De acordo com cada rota da API:
**USUÁRIO :**
* Os vendedores deverão possuir os campos NOME, E-MAIL, PASSWORD e ADMINISTRADOR;
* Não deverá ser possível fazer ações e chamadas para usuários inexistentes;
* Não deve ser possível criar um usuário com e-mail já utilizado;
* Não deverá ser possível cadastrar usuários com e-mails de provedor gmail e hotmail;
* Os e-mails devem seguir um padrão válido de e-mail para o cadastro;
* As senhas devem possuír no mínimo 5 caracteres e no máximo 10 caracteres;
***
**LOGIN :**
* Usuários não cadastrados não deverão conseguir autenticar;
* Usuários com senha inválida não deverão conseguir autenticar;
* No caso de não autenticação, deverá ser retornado um status code 401 (Unauthorized);
* Usuários existentes e com a senha correta deverão ser autenticados;
* A autenticação deverá gerar um token Bearer;
* A duração da validade do token deverá ser de 10 minutos;
***
**PRODUTO :**
* Usuários não autenticados não devem conseguir realizar ações na rota de Produtos;
* Não deve ser possível realizar o cadastro de produtos com nomes já utilizados;
* Não deve ser possível excluir produtos que estão dentro de carrinhos (dependência API Carrinhos);
* Caso não exista produto com o o ID informado na hora do UPDATE, um novo produto deverá ser criado;
* Produtos criados através do PUT não poderão ter nomes previamente cadastrados;

**Riscos:**
* Possível queda de energia ou problema com conexão da internet. Pode ser resolvida com um conexão via celular. 
* Problemas de desempenho durante a manipulação de grandes volumes de dados.

**Divulgação dos Resultados dos Testes:**
   - Um relatório de defeitos será commitado no GitHub nas ISSUES e ser passado no JIRA, para utilizar o board. Este relatório será entregue e apresentado na Sprint3.

**Cronograma:**
    - Início do Projeto: 06/05/2024
    - Período de Testes: 10/05/2024 - 24/05/2024
    - Tabulação dos Dados e Elaboração de Relatórios: 20/05/2024 - 24/05/2024
