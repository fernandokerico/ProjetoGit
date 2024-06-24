### Plano de Testes de Performance

* **Introdução**
  Este documento descreve o planejamento, configuração, execução e análise de um teste de performance realizado na rota `/usuarios` da API ServeRest utilizando o JMeter.

**Escopo:**
- Teste de carga na rota `/usuarios` para medir o tempo de resposta, latência, taxa de erros e throughput.

**Volumetria:**
- Número de usuários planejados: 100
- Número de usuários utilizados na máquina local: 10 (devido às limitações de hardware)

**Métricas a serem acompanhadas:**
- Tempo de resposta
- Latência
- Taxa de erros
- Throughput (requisições por segundo)

#### Execução do Teste
**Análise dos Resultados:**

Tempo de resposta: 21 ms
Latência: 21 ms
Taxa de erros: 0%
Throughput: 10 requisições por 30 segundos (ajustável conforme necessário)

**Observações:**

A rota /usuarios respondeu com sucesso em todas as requisições durante o teste.
O tempo de resposta de 21 ms e a latência de 21 ms estão dentro dos limites aceitáveis para a aplicação.

#### Configuração do Ambiente

Name: Usuários Thread Group
Number of Threads (users): 10
Ramp-Up Period (in seconds): 30
Loop Count: 1
HTTP Request:

Name: Request Usuários
Server Name or IP: localhost
Port Number: 3000
Method: GET
Path: /usuario


**Servidor ServeRest:**
- Executado localmente na porta `3000` com o comando:
  npx serverest@latest

  ### Evidencias:
  * Thread Group
    ![image](https://github.com/fernandokerico/ProjetoGit/assets/139513741/11ebcac4-a27f-43af-8755-4b3b0f548a00)
  * Request usuários
  ![image](https://github.com/fernandokerico/ProjetoGit/assets/139513741/feef40c1-19d2-4ca9-bb56-9ba0b58984c9)
  * View Results Tree
  ![image](https://github.com/fernandokerico/ProjetoGit/assets/139513741/d22f318c-2816-41fa-8fce-4fed695f6e0b)

