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

* Independent (independente) – é uma história que não tem dependências ou amarrações com outras;
* Negotiable (negociável) – não existe um contrato fechado para as definições da história, ela está passível de  conversas e ajustes se necessário, de acordo com uma mudança de contexto ou novas avaliações do time;
* Valuable (valiosa) – sua entrega representa entrega de valor para o usuário final;
* Estimable (estimável) – possui informações suficientes que garantem que o time a compreenda e que seja possível ser estimada;
* Sized-Appropriately/ Small (Tamanho Ideal – Pequena) – é uma história pequena que gera o mínimo de incertezas e que seja possível fazer parte de uma iteração;
* Testable (testável) – seja possível a definição de testes individuais da funcionalidade entregue pela história.

### Critérios de Aceitação (Acceptance Criteria)
Na escrita das histórias, também devemos possuir os critérios de aceitação. Eles são como checklists que devem ser repassados para garantir que aquela história esteja entregando o que foi pedido e planejado em sua definição, em caráter de funcionalidade para entrega de valor ao usuário. Os critérios de aceitação funcionam como uma forma de detalhamento maior sobre o que deve ser entregue naquela história, auxiliando também os desenvolvedores na definição e planejamento dos testes.
####            Exemplo de Cenários com User Storie
``` User Story 

         COMO vendedor```

         EU QUERO visualizar os produtos da loja

         PARA ver sua quantidade em estoque

Descrevendo em formato de tópicos:
O perfil vendedor deve:

ter acesso ao sistema de gestão da loja;
possuir permissão de geração de relatórios;
possuir permissão a opção de relatório ‘’Produtos em Estoque’’.
Descrevendo utilizando cenários:

         Cenário 1: Gerar relatório de Produtos em Estoque

         Dado que o vendedor esteja logado no sistema da loja

             E possua permissão de geração de relatórios

         Quando ele clicar no menu "Relatórios"

            E ser apresentado a opção‘’Relatório de Produtos em Estoque’’

         Então ele deve conseguir gerar o relatório ```