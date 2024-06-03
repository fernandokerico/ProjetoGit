# Curso Testes exploratórios - Udemy

## Automatizado vs Manual
- Testes manuais são mais lentos que os testes automatizados;
- Chega um momento que o  esforço para fazer testes automatizados é muito menor do que o para faazer os manuais
- Testes unitários executam muito rápido, na casa dos milissegundos e o custo é bem menor
- Testes de serviço já chega a 1 segundo ou 2 e o custo é médio
- Testes através da interface chega na casa dos minutos e é maior que 5 segundos e o custo é mais alto
- Testes manuais são bem livres e infinitos

Ambos os testes são importantes e cada um tem uma razão para existir. Enquanto os testes automatizados vão garantir que aqueles roteiros que foram criados vão se repetir a cada execução/commit que for feito e vai garantir que aquilo está funcionando, através dos testes manuais você fica livre para criar novas estratégias e procurar navegar na aplicação com outros olhos.

## Roteiros vs Testes exploratórios
Existe uma pequena diferença entre teste manual/tradicional que tem roteiro de teste e você segue aquele roteiro e vai executando, e isso não é uma exploração, na verdade você está fazendo um script/roteiro.

É interessante fazer testes manuais sem se basear em um roteiro porque:
- Podemos automatizar
- Você está navegando pela aplicação sem uma rota predefinida, sem uma pessoa te ordenando exatamente o que fazer e com isso você tem mais liberdade para prestar atenção

## Automação é nossa amiga
Pode ser utilizada a automação para ajudar nas execuções manuais assim como utilizar as manuais nas automações

## Gerenciamento de massa de dados
Não devemos nos preocupar apenas com entrada e ação, também devemos nos preocupar em como a aplicação está no momento de execução

## Quando parar?
- Deadlines
- Fim dos recursos
- Cobertura de testes atingir a meta
- Taxa de erros reduzir até um determinado patamar
- Alpha/Beta/RC 

## Por onde começar?
Cada aplicação necessita de algo específico então não tem um modelo certo de por onde começar e como exatamente fazer, inclusive se 2 pessoas fizessem o mesmo teste provavelmente elas fariam de formas diferentes (mesmo que não tão diferentes, ainda assim não seria exatamente igual)

## Planejamento de testes
- Planeje antecipadamente (lembrando que não deve ser tão descritivo quanto um caso de teste que fala exatamente tudo que deve ser feito, porém também não deve ser algo totalmente livre, é bom sempre começar com um propósito)
    - Caso de teste >AQUI> ???
    - O que, como, por que? (como; eu quero; para;)
- Crie sessões com tempo pré-determinado
- Evite distrações

## Estratégias iniciais

### Freestyle
Muitas vezes os testes exploratórios são confundidos com testes meio freestyle (que você pega a aplicação entra na home e testa o que quiser). Isso não uma estratégia legal pensando em testes exploratórios. Apesar de ter uma definição abstrata não quer dizer que é vago como um teste ad hoc.

Nesses tipos de teste ad hoc não é seguido nenhum tipo de regra ou padrão, simplesmente vai navegando pela aplicação e fazendo o que quiser/achar que deve. Também não se preocupa com com entradas, com o que está sendo coberto, simplesmente navega e se encontrar algo nesse meio tempo é sorte. Apesar de não ser um teste exploratório não significa que não é utilizado em nenhum momento.

- **Explorar** a aplicação
- **Com** navegação livre
- **Para descobrir** as principais funcionalidades e o fluxo básico do sistema

### Baseado em cenários
Estender cenários existentes, ou seja, pegar um roteiro que já está todo amarrado e a partir daí, vendo a documentação e entendendo, vem ideias de varizações que podem ser feitas nesses roteiros para seguir caminhos diferentes. Então a ideia inicial é uma vez que tenha um caso de uso, entender o fluxo dele e a partir disso fazer algumas variações.

**Variações possíveis de serem feitas**
- Adicionar passos
- Remover passos
- Alterar passos
- Repetir passos
- Substituir passos
- Executar igual, mas diferente

### Baseado em feedback
- Densidade de erros
- Priorização do especialista
- Criticidade de cenários
- Cobertura

### Baseado em técnicas
Combinam a abordagem livre e dinâmica dos testes exploratórios com a estrutura e a sistematização das técnicas formais de teste

### Baseado em equivalência
Tem o objetivo de reduzir o número de casos de testes necessários por meio do agrupamento de entradas que devem ser tratadas da mesma forma pelo sistema em classes de equivalência. Essa abordagem se baseia principalmente na ideia de que se um valor em uma classe de equivalência é processado corretamente pelo sistema, todos os outros valores dessa classe também são

### Classe de equivalência
Tenta mapear um conjunto infinito de possibilidades em um subconjunto finito bem menor para conseguirmos testar

### Valor Limite
Ele é meio que um complemento para as classes de equivalência porque ele diz que devemos pegar os elementos que estão bem na fronteira entre uma classe e outra

### Transição de estados
É uma técnica muito boa para quando a funcionalidade/módulo que for ser testado pdoe ser mapeada em uma máquina representada como se fosse uma máquina de estados. Deve ter um número finito de estados, devemos conseguir saber exatamente que ação leva a cada estado

### Tabela de decisão
Quando o conjunto de regras e o conjunto de resultados está mais extenso, aí precisamos desenhar/representar de alguma forma e uma boa forma de fazer isso é utilizando a tabela de decisão. 

### Array ortogonal
Essa estratégia consiste em reduzir um conjunto maior em um conjunto muito menor (no caso de uma tabela de decisão muito grande esse funcionaria melhor)

## Personas
Personas é uma ferramenta que vai ajudar a conscientemente adotar habitos e pensamentos de outras pessoas. Persona é uma forma de tentar agrupar essa "população mundial" em pequenos grupos. Uma estratégia mais interessante seria mapear os tipos/perfil dos usuários e a partir disso criar uma persona para cada um desses tipos e começar a pensar como essas pessoas iriam utilizar a aplicação.

- Dar um nome de fácil relação com o perfil
- Criar um breve background
- Levantar um conjunto de características
- Anexar uma fotografia ajuda a fixar melhor
- Mapear os hábitos e necessidades da persona e como ela poderia interagir com o sistema

## Soap Opera Scenarios

### Soap Opera Testing
Quando é criado cenário baseado em Soap Opera todas as funcionalidades vão meio que funcionar ao mesmo tempo, esse registro vai sendo evoluído ao longo dessa história/roteiro que vamos criar. Criar cenários mais elaborados e que tentam agrupar maior quantidade de cenários possíveis. 

- Testes devem ser engraçados e agressivos
- Escreva cenários improváveis, mas possíveis
- Escreva cenários exagerados e condensados
- Possui fase de design e execução separadas

## Turismo

### Tours
Essa questão de turismo de cidades/países pode ser trazida para os testes também. Existem pessoas que planejam tudo que vão fazer antes da viagem (criam um roteiro) e existem pessoas que não planejam nada e só vão. Da mesma forma acontece nos testes e seus tipos.

### Business District
- **Guidebook Tour:** Nos testes um ótimo gruia é o manual da aplicação. Quando o manual descreve uma funcionalidade e como ela deve funcionar, o testador automaticamente já vai saber exatamente o que testar e como a aplicação deve se comportar. Defeitos encontrados nessa rota normalmente possuem prioridade alta.
- **Money Tour:** Precisamos tentar identificar a razão principal pela qual os usuários utilizam a aplicação porque se essa parte principal para de funcionar, ninguém mais vai querer usar ela.
- **Landmark Tour:** Nos testes escolher pontos de aplicação que deseja visitar e montar uma rota que passe por todos eles. Manter um registro dos pontos visitados para ter uma noção de quais já foram cobertos.
- **FedEx Tour:** Nos testes identificamos entradas que são armazenadas no sistema e procurar segui-las pelo software.
- **After-Hours Tour:** Nos horários que as funcionalidades mais importantes não são utilizadas em larga escala, algumas outras funcionalidades podem ser acionadas e é nesse ponto que podemos tentar fazer a execução de tarefas agendadas para rodar durante a noite ou fazer backup etc, depende do que a aplicação precisa.
- **Garbage Collector's Tour:** Nos testes, quando queremos verificar as interfacesnós visitamos tela por tela, mensagem por mensagem sempre buscando a menor rota possível e nunca parando em algum outro detalhe do teste.

### Historic District
A região histórica é aquela que cuida de código legado e funcionalidades que já existiam previamente

- **Bad Neighborhood Tour:** Áreas infestadas de bugs e que o testador é orientado a ficar a maior quantidade de tempo possível.  
- **Museum Tour:** Nos testes, as intimidades são os códigos legados que muitas vezes quando olhamos parece que foi feito por um artista. Após a saída dos desenvolvedores originais do código geralmente com uma documentação defasada esses códigos são extremamente difíceis de entender, manter e até emsmo criar testes para eles. Então os testadores devem identificar esses blocos de código, esses módulos que existem e dar atenção as funcionalidades que exercitam esses códigos.
- **Pior Version Tour:** Os testadores devem tentar garantir que uma funcionalidade apesar de que ela tenha sido atualizada, não tenha perdido a sua essência.

### Entertainment District
- **Supporting Actor Tour:** Nos testes, vamos focar nas funcionalidades que dividem a tela com as principais  funcionalidades da aplicação. 
- **Back Alley Tour:** Nos testes visite aquelas funcionalidades que raramente alguém vai utilizar.
- **All-Nighter Tour:** Nos testes poderiamos manter a aplicação rodando sem fechá-la, deixar a noite toda rodando, deixar ela aberta e ver como ela se comporta, como ela faz o gerenciamento de memória, se o token de acesso deveria durar tanto tempo, se aparece mensagem amigável ou trava tudo, etc

### Tourism District
- **Collector's Tour:** Nos testes, tente mapear todos os testes e vá catalogando as visitas a medida que elas ocorrem
- **Lonely Businessman Tour:** Nos testes, procure as funcionalidades que estão mais distantes do ponto inicial da aplicação, qual funcionalidade necessita de mais cliques para chegar nela, aplica garbage collector também no caminho.
- **Supermodel Tour:** Nesses testes você deve ser superficial. Não tente se aprofundar muito nos testes, o importante aqui é a apresentação e as primeiras impressões, então foque apenas nas interfaces. Veja se elas estão boas, se estão renderizando corretamente, se demoram muito para aparecer, etc

### Hotel District
- **Rained-Out Tour:** Nos testes o foco seria em iniciar operações e cancelá-las logo em seguida, caso não tenha botão de cancelar tentar clicar no esc ou até fechar o browser ou aplicação e verifique o comportamento
- **Couch Potato Tour:** Nos testes, tente passar pelas funcionalidades sempre com valores default, se existe alguma informação obrigatória faça o mínimo necessário.

## Outras estratégias

### Shoe Test 
Essa estratégia diz exatamente o que dá a entender pelo nome, que voce vai pegar um sapato e espancar o teclado com ele. O motivo seria que foram percebidas que algumas aplicações trazem um comportamento estranho quando você aperta diversas teclas de uma vez. Também tem a opção mais "higiênica" que seria utilizar livros ao invés de sapatos

### Null, Zero, Vazio
É basicamente tentar como entrada tudo que for possível: null, zero, vazio, espaço, negativo, etc. 

### Get one, take one
Consiste em abrir 2 instâncias da aplicação quando ela trabalha com recursos e ver se o fato de estar trabalhando de um lado acaba atrapalhando o outro lado

### Bookmark
Em aplicações web tem o link/url da aplicação e dependendo de como você vai navegando na aplicação essa url vai mudando, e muitas vezes temos costume de armazenar esse link ou salvar em um bloco de notas ou algo do tipo e depois tentar acessar a aplicação diretamente nessa url e ver como ela se comporta.

### Sabotage
Entender o funcionamento da aplicação, entender quais são as dependências que ela possui e tentar retirá-las e ver como a aplicação vai se comportar nesses casos.

### Responsividade e Acessibilidade
Para uma aplicação ser considerada responsiva, ter um layout responsivo quer dizer que independente da resolução da tela, do tamanho que tem disponível na tela, os elementos dela vão se adequar para que você consiga trabalhar bem com eles.

Pensando em acessibilidade, que seria como que uma pessoa que tem alguma necessidade especial poderia interagir com sua aplicação, aí depende muito da necessidade que a pessoa tem. E não necessáriamente você precisa ter uma necessidade especial para que uma aplicação atrapalhe sua experiência

### Segurança
Como proteger a aplicação de ataques; Segurança é uma linha tênue entre pessoas tentando garantir a segurança e pessoas descobrindo as falhas de segurança de forma maliciosa

---
# Gostaria de agradecer e referenciar minha colega **Mariana Cristina da Silva Teixeira** que cedeu suas anotações para mim! Por conta do tempo, acabei conseguindo apenas assistir ao curso. 