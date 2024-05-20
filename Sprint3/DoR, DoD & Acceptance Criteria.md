# User Story
    A escrita das histórias de usuário funcionam como uma narrativa sobre o quê, para quem e porque entregar aquela funcionalidade. É um direcionador ao desenvolvimento!

#### Template para escrita de User Story
    
 * __Como__ – autor da ação (persona);
 * __eu quero__ – funcionalidade desejada;
 * __para__ – valor agregado à funcionalidade desejada.

#### Técnica 3W 
`Na utilização dessa técnica devemos nos atentar a quem é o nosso sujeito ou usuário, ou seja, como o usuário se encontra (persona), o que ele deseja realizar e para quê ou porquê ele deseja executar aquela atividade ou ação. `

Seguindo o modelo apresentado acima temos:

* Como (quem?) – aqui eu devo referenciar para quem eu estou construindo aquela funcionalidade. Quem é a minha persona atingida por aquela história?
* eu quero (o quê?) – aqui eu devo colocar qual a funcionalidade esperada. O que minha persona deseja realizar?
* para (por quê?) – devo descrever qual a motivação para a construção daquela história. Qual o valor esperado pela pessoa usuária?

#### Técnica 3C 
Esta técnica nos trás para uma preocupação com o conteúdo dos questionamentos da técnica do 3W. Os 3C representam card (cartão)/ conversation (conversa)/ confirmation (confirmação), onde:

* Cartão – uma User Story não deve ser muito extensa, tornando possível escrevê-la em um único cartão;
* Conversa – seu conteúdo deve gerar discussões de alinhamento entre o time sobre o que se deseja atender;
* Confirmação – é importante que a história de usuário possua critérios de aceitação para que seja possível a validação de êxito na construção e entrega.
#### Técnica INVEST
Preocupado com a escrita de histórias de usuário, William C. Wake, em seu livro Extreme Programming Explore, criou o acrônimo INVEST. Nele temos as seis principais características a serem consideradas na criação, definição e escrita de uma história de usuário, que são:

![Modelo INVEST](https://miro.medium.com/v2/resize:fit:520/format:webp/0*vuw5VxQSXzodFoGf.) 

* Independent (independente) – é uma história que não tem dependências ou amarrações com outras;
* Negotiable (negociável) – não existe um contrato fechado para as definições da história, ela está passível de  conversas e ajustes se necessário, de acordo com uma mudança de contexto ou novas avaliações do time;
* Valuable (valiosa) – sua entrega representa entrega de valor para o usuário final;
* Estimable (estimável) – possui informações suficientes que garantem que o time a compreenda e que seja possível ser estimada;
* Sized-Appropriately/ Small (Tamanho Ideal – Pequena) – é uma história pequena que gera o mínimo de incertezas e que seja possível fazer parte de uma iteração;
* Testable (testável) – seja possível a definição de testes individuais da funcionalidade entregue pela história.

### Critérios de Aceitação (Acceptance Criteria)
Na escrita das histórias, também devemos possuir os critérios de aceitação. Eles são como checklists que devem ser repassados para garantir que aquela história esteja entregando o que foi pedido e planejado em sua definição, em caráter de funcionalidade para entrega de valor ao usuário. Os critérios de aceitação funcionam como uma forma de detalhamento maior sobre o que deve ser entregue naquela história, auxiliando também os desenvolvedores na definição e planejamento dos testes.
####            Exemplo de Cenários com User Storie
* User Story 

         COMO vendedor

         EU QUERO visualizar os produtos da loja

         PARA ver sua quantidade em estoque

Descrevendo em formato de tópicos:
O perfil vendedor deve:

ter acesso ao sistema de gestão da loja;
possuir permissão de geração de relatórios;
possuir permissão a opção de relatório ''Produtos em Estoque''.
* Descrevendo utilizando cenários:

         Cenário 1: Gerar relatório de Produtos em Estoque

         Dado que o vendedor esteja logado no sistema da loja

             E possua permissão de geração de relatórios

         Quando ele clicar no menu "Relatórios"

            E ser apresentado a opção‘’Relatório de Produtos em Estoque’’

         Então ele deve conseguir gerar o relatório 

*   

 ### DICAS:
* **Utilize o acrônimo INVEST** – isso garantirá que sua história esteja o mais completa possível, possibilitando maior entendimento do seu time, eliminando, assim, possíveis falhas ou retrabalho.
* **Liste os critérios de aceitação** – sempre tenha definido quais são as condições, restrições e as regras de negócio do produto.
* **Descreva os cenários** – Utilize a técnica BDD para descrever os cenários daquela história. É importante que os cenários de testes sejam mapeados, em âmbito de negócio e comportamento.

# Definition of Ready (DoR)
- ⭐️Defintion of Ready (DoR) é um acordo de trabalho entre o time de Desenvolvimento e o Product Owner, aplicado a **todas** as Histórias de Usuário, com a intenção de que os itens do Backlog não cheguem para a reunião de planejamento com granularidade ruim, pouco ou nenhum detalhamento.
- É preciso disciplina para reservar até 10% do tempo da Sprint para que o Product Backlog seja preparado adequadamente com a finalidade de reduzir o impacto de itens mal especificados, que muitas vezes fazem com que os times façam um planejamento de baixa qualidade, gerando necessidade de mudanças na implementação e impactando os objetivos da sprint.

# Definition of Done (DoD)
- ⭐️Definition of Done (DoD) é um acordo, definido pelos membros do time Scrum (Desenvolvedores e Product Owner), aplicável a **todas** as Histórias de Usuário, com o intuito de que todos os membros do time tenham um entendimento compartilhado do que significa “Done” para garantir a transparência. Ou seja, uma lista de verificação de atividades necessárias para que um incremento de software seja considerado como **completo.**

# Critérios de Aceite
- ⭐️Já, os critérios de aceite são específicos e diferentes para diferentes Histórias de Usuário. É uma lista de critérios que precisam ser alcançados para que a User Story atenda os requisitos do usuário e seja aceita pelo Product Owner. Os critérios de aceitação contém informações adicionais que não foram inseridas nas users stories para não poluir o corpo principal do texto.
![ ](https://miro.medium.com/v2/resize:fit:484/format:webp/0*9OloFpb8XmicmmKX.) 

#####  Os critérios de aceitação têm o objetivo de:
* Definir limites para as user stories
* Ajudar o P.O. a detalhar em alto nível o que é necessário para entregar valor ao cliente
* Ajudar o time a entender melhor o objetivo da user story
* Ajudar programadores e testadores a planejarem os testes
* Informar ao programador quando parar de adicionar funcionalidades à user story
##### O que são bons critérios de aceitação?
* São escritos com menor nível de detalhamento
* São independente de implementação
* Definem o que fazer e não como fazer

### Exemplos de Critérios de Aceitação

**User Story**

* Como um operador de marcação de consulta
* Eu gostaria de visualizar a agenda de consultas dos médicos
* Para saber quais horários estão disponíveis para novas marcações.

**Critérios de aceitação**
* Eu quero ter opções de visualização da agenda por dia, semana e mês.
* Eu quero visualizar a agenda de consultas do mês atual e do mês posterior.
* Cada consulta agendada deve mostrar o nome e o convênio do paciente

# **__________________________________________________________________________**
*** 
* **⟹ Quando o time deve criar a sua DoR e DoD?**
Idealmente, o time deve criar antes da primeira sprint. Porém, caso o seu time ainda não tenha uma definição de ready e/ou done criada, ou que não esteja clara para todos, uma boa oportunidade é levantar o assunto sobre a oportunidade de criarem a sua DoR e/ou DoD durante a retrospectiva.

* **⟹ Uma vez criada a DoR e DoD, elas nunca mais poderão ser alteradas?**
Elas poderão ser alteradas sempre que fizer sentido para o time. Utilize a retrospectiva para inspeção e adaptação.

* **⟹ Cada time deve ter a sua própria DoR e DoD?**
Idealmente sim, cada time cria seus próprios critérios de pronto, embora muitas vezes alguns itens da DoR e DoD possam ser similares a todos os times por ser algum requisito da área/setor/empresa.

* **⟹ De quem é a responsabilidade de tornar o item “Ready”?**
É de responsabilidade do Product Owner, embora ele(a) possa envolver outras pessoas do time nessa atividade.

* **⟹ Quando deve ser feito o trabalho de refinamento para deixar os itens**“Ready”?
Idealmente, na Sprint anterior a que se deseja incluir o item.

# ÉPICO
* Um Épico é uma User Story muito grande que levaria mais de um sprint para ser desenvolvida. Um Épico deve ser quebrado em User Stories menores que possam ser desenvolvidas em um sprint.

![ ](https://miro.medium.com/v2/resize:fit:720/format:webp/0*cmmbSRHmW5UAbuCp.) 

* Exemplo de Épico: como cliente do banco desejo consultar e movimentar meus produtos.

* Poderíamos quebrá-lo nas seguintes User Stories:

**Como** cliente do banco **desejo** consultar o extrato da minha conta corrente **para** verificar meu saldo e os lançamentos realizados.
**Como** cliente do banco **desejo** consultar a fatura do meu cartão de crédito **para** saber quanto terei que pagar.
**Como** cliente do banco **desejo** realizar o pagamento de um boleto **para** quitar uma conta.
**Como** cliente do banco **desejo** agendar uma transferência de dinheiro mensalmente da minha conta corrente **para** a poupança, para garantir o cumprimento da minha meta de economia no mês.

