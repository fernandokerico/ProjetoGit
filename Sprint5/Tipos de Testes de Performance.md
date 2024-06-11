### Princípios do Teste de Performance

O teste de performance é vital para assegurar a qualidade dos aplicativos e a satisfação do usuário. Esta avaliação avalia a funcionalidade, usabilidade e outras características de qualidade sob diferentes cargas, revelando possíveis problemas. O teste de performance é relevante para várias arquiteturas de sistemas, não se limitando a aplicações web.

A eficiência de performance é categorizada na ISO-25010 como uma característica de qualidade não funcional, que inclui três subcaracterísticas:

**Comportamento do tempo:** Avalia o tempo de resposta de um componente ou sistema às entradas do usuário ou do sistema.

**Utilização de recursos:** Investiga a alocação e utilização dos recursos do sistema, como a memória RAM.

**Capacidade:** Avalia o comportamento do sistema nos limites de sua capacidade, como número de usuários ou volumes de dados.

Os testes de performance assumem a forma de experimentação, podendo ser conduzidos iterativamente para suportar a análise, design e implementação do sistema.

**Os princípios importantes dos testes de performance são**:

* Alinhamento com as expectativas dos stakeholders.
* Reprodutibilidade dos testes.
* Produção de resultados compreensíveis e comparáveis.
* Execução em sistemas completos ou parciais ou em ambientes similares ao de produção.
* Praticidade, acessibilidade e execução dentro do prazo do projeto.
* Estes princípios e subcaracterísticas ajudam a dimensionar a capacidade do sistema em teste (SUT) e formam a base para os testes de performance, conforme destacado pelos livros de [Molyneaux09] e [Microsoft07].

### Tipos de Teste de Performance​​​​​​​

Os diferentes tipos de testes de performance são adequados para diferentes projetos, dependendo dos objetivos do teste:

**Teste de Performance:** Este é um termo genérico que se refere a qualquer tipo de teste focado na performance do sistema ou componente sob variados volumes de carga.

**Teste de Carga:** Este teste foca na habilidade do sistema de lidar com níveis crescentes de carga, geralmente oriundos de um número aumentado de usuários ou processos.

**Teste de Estresse:** Este tipo de teste avalia a capacidade do sistema de lidar com picos de carga que ultrapassam os limites previstos de carga de trabalho. Ele também testa a resistência do sistema a uma diminuição de recursos disponíveis.

**Teste de Escalabilidade:** Este teste mede a capacidade de um sistema de atender a requisitos futuros de eficiência, incluindo expansão para mais usuários ou grandes quantidades de dados.

**Teste de Pico:** Avalia a capacidade do sistema de lidar com rajadas súbitas de cargas de pico e retornar a um estado estável.

**Teste de Resistência:** Este tipo de teste foca na estabilidade do sistema ao longo de um período específico, verificando se não há problemas que possam degradar a performance ou causar falhas ao longo do tempo.

**Teste de Concorrência:** Este teste verifica o impacto de ações específicas que ocorrem simultaneamente, como quando muitos usuários fazem login ao mesmo tempo.

**Teste de Capacidade:** Este teste determina o número de usuários e/ou transações que um sistema pode suportar, mantendo uma performance aceitável.

Esses testes são essenciais para garantir que um sistema possa lidar com diferentes cargas e situações, mantendo uma performance consistente e estável.

### Testando os tipos do Teste de Performance​​​​​​​

Os testes de performance são cruciais para garantir a eficácia e eficiência de um sistema. Eles podem ser classificados em testes estáticos e testes dinâmicos.

**Testes Estáticos:** Envolvem a análise da performance do sistema sem executar o programa. Eles são especialmente úteis para detectar problemas de performance que podem ocorrer durante a modelagem e arquitetura do sistema. Os testes estáticos incluem revisões de requisitos, análise do banco de dados e esquemas de redes, e revisões do código do sistema.

**Testes Dinâmicos:** Estes são conduzidos enquanto o sistema está em execução. Podem ser realizados em vários estágios do ciclo de vida do desenvolvimento do software, incluindo o teste de unidade, teste de integração de componentes, teste de sistema e teste de integração do sistema. É importante para os testes de performance serem incorporados ao ciclo de vida iterativo do desenvolvimento do software desde o início. O teste de performance dinâmico também pode ser realizado usando simuladores, embora seja ideal testar o hardware real o mais cedo possível.

**Geração de Carga:** Para a realização de vários tipos de testes de performance, é necessário modelar, gerar e submeter cargas representativas ao sistema em teste. As cargas podem ser geradas de várias maneiras:

**Geração de Carga através da Interface do Usuário:** Adequada quando apenas um pequeno número de usuários precisa ser representado. No entanto, essa abordagem pode ser limitada quando o número de usuários a serem simulados aumenta.

**Geração de Carga usando Grupos:** Envolve muitos testadores que representam usuários reais. Essa abordagem é útil para testar aplicações acessíveis globalmente, mas a carga gerada pode não ser tão precisa ou reprodutível.

**Geração de Carga por meio de API (Application Programming Interface):** Permite simular a interação do usuário com o sistema em teste de uma maneira menos sensível a alterações na interface do usuário. Scripts dedicados podem ser criados para chamar rotinas API específicas.

**Geração de Carga usando Protocolos de Comunicação Capturados:** Involui a captura da interação do usuário com o sistema em teste no nível do protocolo de comunicação e reprodução desses scripts para simular um grande número de usuários.

Esses testes são fundamentais para garantir que o sistema pode lidar com diferentes cargas e condições enquanto mantém uma performance consistente e estável.

#### Modos comuns de falha de eficiência de performance e suas causas

Durante testes dinâmicos, alguns problemas comuns de desempenho podem surgir, incluindo:

**Resposta lenta em todas as cargas:** Pode ser causado por problemas subjacentes como modelagem inadequada do banco de dados, latência de rede e outras cargas de fundo.

**Resposta lenta sob carga moderada a pesada**: A resposta pode se degradar de forma inaceitável com cargas dentro dos limites permitidos. A causa geralmente é a saturação dos recursos ou variações de cargas pesadas.

**Resposta degradada ao longo do tempo:** Este é um problema em que a resposta se degrada gradualmente com o tempo. Causas típicas incluem vazamentos de memória, fragmentação de disco, aumento da carga de rede, crescimento do repositório de arquivos e crescimento inesperado do banco de dados.

**Tratamento inadequado de erros sob alta carga ou além do limite:** Aqui, o tempo de resposta é aceitável, mas o tratamento de erros é inadequado em altos níveis de carga. Defeitos subjacentes comuns incluem recursos insuficientes, filas e pilhas pequenas e configurações de tempo limite muito rápidas.

Exemplos específicos desses problemas incluem um aplicativo web que não responde dentro de um prazo aceitável, um sistema que falha sob uma grande quantidade súbita de solicitações, sistemas que apresentam resposta lenta quando lidam com grandes volumes de dados, processamento em lote que não pode ser concluído a tempo e sistemas em tempo real que ficam sem memória suficiente ao lidar com grandes demandas de memória dinâmica.


