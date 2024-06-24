# TESTES DE PERFORMANCE

#### Habilidade para se tornar Analista de QUALIDADE
* Boa comunicação;
* Saber Ouvir;
* Se adaptar;
* Pensamento crítico;
* Tomar decisões;

#### Qual importancia desses requisitos de performance?
* Prevenção de problemas;
* Direcionamento para desenvolvimento;
    - Guiar arquitetura para atender necessidades dos clientes
* Visibilidade do impacto no negocio
    - Janelas de processamento
    - Visão sistemica da funcionalidade
* Evitar
    - Retrabalhos
        -Custos:
            - Horas ou Financeiros
    - Restruturação na arquitetura  da aplicação
    - Stress com clientes/usuários
    - Perda financeira com cliente
    - Reputação da aplicação
        - Exposição negativa em redes sociais
    - Problemas de responsabilidade legal

###### O que é teste de performance?
* Quantidade de usuários simultaneos
- Tenpo de resposta e de processamento
* O objetivo é medir:
    * desempenho;
    * capacidade;
    * confiabilidade;
    * disponibilidade
    * escalabilidade
    * resiliencia;
    * **Utilização de recursos**
        Consumo de memória
        Consumo de CPU
        Espaço em disco
* **EXPERIMENTAÇÕES**
    * Eliminar obstaculos de desempenho
    * Entender melhores configurações
    * Entender necessidades de hardware para atender os requisitos de performance

* **Principios**
* Alinhado as expectativas de todos envolvidos
* Entender:
    * Objetivo: Qual a necessidade de performance?
    * Contexto:
        * Negocio
        * Técnico
    * Risco:
        * Criticidade
    * Escopo
    * Não escopo
    * Critérios de aceite
        * Definição de métricas

##### Reprodutiveis
 **MASSA DE DADOS**
* Criada em tempo de execução
* Geração de carga
* Duplicidade
* Configurações
* Inconcistencia com negócio
* valores válidos
* pré-cadastrada

###### RESULTADOS COMPREENSÍVEIS:
**Status de acordo com as expectativas dos stakeholders:**
* Passou
* Falhou
* Evidencias

**Linguagem entendida por todos os stakeholders**
* Negócio
* Técnica
---
## Quais são os tipos de testes de performance?
* Testes de performance
    * Termo abrangente
    * Genérico para qualquer tipo de teste de desempenho
    * Cada tipo de teste tem um objetivo diferente
    * Importante lembrar:
        * De acordo com o contexto pode ser que precise aplicar mais de um tipo de teste

* Carga ou volume
    * **objetivo**
        * Avaliar a aplicação quando o sistema é submetido a aumento de carga
            * Níveis crescentes de cargas
            * Usuários simultaneos (threads)
            * Quantidade de registros

* Capacidade
    * **objetivo**:
        * Avaliar e descobrir o limite da aplicação
            * **Aumento de carga**
            * Níveis crescentes de cargas
            * Usuários simultaneos (threads)
            * Quantidade de registros

* Escalabilidade
    * objetivo
        * avaliar a capacidade do sistema de expandir

* Stress
    * Avaliar comportamento da aplicaçãp com cargas próximas/superiores limite
        * Aumento de carga acima do limite/pico
            * Usuários simultaneos (threads)
            * Quantidade de registros
        * Pior cenário (relacionado volume)
            * disponibilidade
            * resiliencia
            * recuperação

* Pico
    * objetivo
        * Avaliar comportamento da aplicação  após rajadas repetinas
            * Grande quantidade de threads simultaneas em determinao tempo
            * estabilidade
            * disponibilidade

* Resistencia
    * objetivo
        * avaliar comportamento da aplicação com maior volume em periodos mais longos
        * degradação da performance
            * Hardware
            * Aplicação
        * Falhas
        * Interrupções

* Concorrencia
    * objetivo
        * Avaliar impactos na aplicação em execuções simultaneas]
        * dificil de reproduzir

* Ramp-up
    * Steps
    * subida gradativa de carga
    * facilita encontrar momento de ruptura
---
#### **Quais metricas podemos utilizar?**
* Tempo de resposta 
    * unidade de tempo (minuto, milisegundos,  segundos)
* Média do tempo de resposta (porcetagem)
* Throughtput
   * Transação por segundo (TPS)
* Latencia: Atraso (o tempo) que uma solicitação leva para ser transferida de um ponto para outro
##### FALHAS COMUNS
* Resposta lenta sob todos os niveis de carga
    * Implementação
    * modelagem
    * latencia
* Resposta lenta sob níveis de carga moderada a pesada
    * Itens acima
    * recursos de hardware
* Resposta degrada ao longo do tempo
    * Vazamento de memória
    * Aumento de carga de rede ao longo do tempo
    * gravação  em disco
* Tratamento inadequado de erros sob carga pesada ou acima do limite
    * Divergencia de configurações
    * timeout
    * funcional
## Hardskills para performance
* Conceito de banco de dados
* Conceitos de performance e testes de performance (estratégias)
* aprofundar na arquitetura da aplicação
* analisar métricas para construção de relatórios
* conhecer alguma linguagem para aplicar no script

#### Processos de testes de performance
* Maior desafio/duvidas
    * Como encontrar métricas?
    * entender como análise de dados
* Sugestoes de implementação
    * Pré-requisitos
        * Priorizar --> Selecionar as principais funcionalidades
        * Definir métricas
            * Classificar numeros entre x e y ou até z tempos
                * Escala:
                    * Ruim
                    * Aceitável
                    * Bom
                    * Excelente
                * Exemplo:
                    * Ruim Acima de 3s
                    * Aceitável 2 a 3s
                    * Bom 1 a 2s
                    * Excelente Abaixo de 1s

        * ambientes
        * Ferramentas
            * JMeter
    * Estrutura:
        * Shift left testing de performance
        * Entendimetno da demanda
        * criação de scripts
        * execução de testes
        * Análise dos insumos coletados no teste

        # JMETER
        Apache JMeter
        open source 100% em Java.