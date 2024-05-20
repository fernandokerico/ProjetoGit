# Jira
* Criado em 2002 para rastreamento de bugs, gerenciamento de projetos e issues.
***
##### Tipos de Jira: Bug ou Issue de aceitação
* Quando estamos homologando o sistema criamos bugs para os problemas localizados durante a homologação. Durante a etapa de aceite o cliente vai abrir também solicitações do tipo bug para verificação. Podemos ativar no jira para essas solicitações do cliente o tipo issue de aceitação, assim fica mais fácil a rastreabilidade do que foi aberto pela equipe interna Compass ou cliente.
##### Como identificar uma solicitação do cliente:
***O problema encontrado é um bug ou uma melhoria?***

* Para responder a esse questionamento, lembre-se sempre que a melhoria deve ser sugerida para proporcionar algum benefício no software, enquanto o erro impactará na obtenção de um resultado diferente do esperado. Uma melhoria deverá ser avaliada pela gestão do projeto para verificação se será ou não implementada nessa etapa.

***
#### Como classificar bug em dev/análise/massa/ambiente


**Os bugs podem ocorrer devido a vários motivos e devemos localizar a causa raiz.**

* **DEV:** O bug pode ter ocorrido devido a uma falha no desenvolvimento da demanda.

* **ANÁLISE:** Especificações funcionais e técnicas elaboradas erroneamente ou que não suprem a necessidade do cliente.

* **MASSA:** Inconsistência nos dados utilizados para testes.

* **AMBIENTE:** Falha no ambiente que está sendo utilizado para testes. Nesse caso pode ser necessário entrar em contato com a fornecedora do produto ou administrador do sistema

***
### Estratégias de Testes

##### Tipos de Issues
* **Melhoria**: É quando um determinado requisito é identificado no sistema que ainda não está implementado mas pode ser implementado para gerar um benefício ao cliente. Por exemplo, o sistema, hoje, gera relatórios com informações baseadas na data escolhida pelo o usuário. Mas poderia existir a opção de escolher a data e o local.
* **BUG**: É quando uma determinada funcionalidade do sistema não está funcionando como foi definido pelo o cliente. Por exemplo, o botão salvar não está executando nenhuma ação ao clicar. Ou, uma determinada tela do sistema não está sendo carregada conforme o layout especificado pelo cliente.

#### Status de Execução de um Caso de Teste:
* **Aberto:** Caso de teste criado que ainda não foi executado.
* **Em execução:** Está sendo executado (testado).
* **Passou:** Foi executado e está sem bugs abertos vinculados ao fluxo.
* **Falhou:** Foi executado sendo encontrado bugs no fluxo (Todo status de falha deverá estar vinculado ao bug criado durante a execução).
* **Bloqueado:** Alguma ação externa está bloqueando a execução do fluxo. Ex: Massa de dados específica que dever´ser entregue pelo cliente, como cpf,cnpj de usuário da loja que possua algum dado que não conseguimos criar através da nossa aplicação e que só existe na base do cliente.
* **Cancelado:** Não será executado, geralmente ocorre quando a funcionalidade foi retirada do escopo do projeto.

##### Report de Testes


***
##### GESTÃO DE DEFEITOS NOS TESTES DE SOFTWARE

```O grande objetivo do Teste é garantir qualidade ao sistema.```

###### Processo de Gestão de Defeitos
![ERRO,, DEFEITO E FALHA](https://arquivo.devmedia.com.br/REVISTAS/java/imagens/94/7/image001.jpg)

**A explicação de cada conceito é resumida em:**

**Erro _(engano):_** ação humana que produz resultados incorretos, como por exemplo, a implementação errada de um algoritmo;
**Defeito _(bug):_** falha em um sistema que pode ocasionar uma anomalia ao tentar desempenhar sua devida função. Por exemplo, omissão de informações e cálculos incorretos;
**Falha:** ação inesperada no software. Por exemplo, o sistema apresenta resultados diferentes do planejado.

* O problema encontrado é um **defeito** ou uma **melhoria**? Para responder a esse questionamento, lembre-se sempre que a **melhoria** deve ser sugerida para proporcionar algum benefício no software, enquanto o **erro** impactará na obtenção de um resultado diferente do esperado;
* **O quão crítico é o bug?** Cada bug encontrado deve ser classificado de acordo com a sua criticidade. Para isso, é essencial definir qual será o impacto no projeto caso o problema não seja resolvido;