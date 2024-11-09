
## Introdução

Este script tem o objetivo de simular cenários de atendimento ao cliente, calculando KPIs que oferecem uma visão sobre a eficiência das ligações telefônicas e a curadoria de chatbots. Essa análise é útil para empresas que buscam otimizar seus processos de atendimento e melhorar a experiência do cliente.

---

## KPIs Medidos

### Ligações Telefônicas

1. **Tempo Médio de Atendimento (TMA)**: Média de tempo gasto em atendimento.
2. **Tempo Médio de Espera (TME)**: Média de tempo que o cliente aguarda para ser atendido.
3. **Taxa de Abandono de Ligações**: Porcentagem de ligações que foram abandonadas antes de serem atendidas.
4. **Taxa de Resolução na Primeira Chamada (FCR)**: Porcentagem de chamadas resolvidas sem a necessidade de uma nova chamada.
5. **Nível de Satisfação do Cliente (CSAT)**: Média de satisfação dos clientes, variando de 1 a 5.
6. **Taxa de Transferência**: Porcentagem de ligações transferidas para outro atendente.
7. **Análise de Sentimento**: Distribuição de sentimentos (Positivo, Neutro, Negativo) das ligações.

### Curadoria de Chatbot

1. **Taxa de Resolução Automatizada**: Porcentagem de interações resolvidas automaticamente pelo chatbot.
2. **Taxa de Fallback**: Porcentagem de interações que resultaram em fallback (quando o chatbot não conseguiu responder).
3. **Tempo Médio de Resposta do Chatbot**: Média de tempo de resposta do chatbot em segundos.
4. **Taxa de Engajamento**: Percentual de usuários que interagiram ativamente com o chatbot.
5. **Índice de Satisfação do Chatbot (CSAT)**: Média de satisfação dos usuários com o chatbot, variando de 1 a 5.
6. **Análise de Intenções Não Reconhecidas**: Porcentagem de intenções que o chatbot não conseguiu identificar.
7. **Taxa de Transferência para Atendente Humano**: Porcentagem de interações transferidas para um atendente humano.

---

## Requisitos

- **Python 3.7+**
- **Bibliotecas**:
  - `random`
  - `pandas`

---

## Instalação das Bibliotecas

Para instalar as dependências necessárias, execute o comando a seguir para instalar o `pandas`:

```bash
pip install pandas
```

---

## Como Executar

Para executar o script:

1. Clone este repositório ou copie o script Python.
2. Instale as dependências necessárias.
3. Execute o script com o comando:

```bash
python medir_kpis.py
```

---

## Estrutura do Código

- **Função `generate_call_data(num_calls)`**: Gera um dataset fictício para simular dados de ligações telefônicas.
- **Função `generate_chatbot_data(num_interactions)`**: Gera um dataset fictício para simular dados de interações com o chatbot.
- **Cálculo dos KPIs**: Os KPIs são calculados utilizando métodos de agregação, como média e contagem, aplicados aos dados gerados.

---

## Exemplo de Saída

O script gera uma saída com os KPIs calculados para ligações telefônicas e interações com o chatbot. Exemplo:

### KPIs para Ligações Telefônicas

- **Tempo Médio de Atendimento (TMA)**: 9.87 minutos
- **Tempo Médio de Espera (TME)**: 4.32 minutos
- **Taxa de Abandono de Ligações**: 42.50%
- **Taxa de Resolução na Primeira Chamada (FCR)**: 58.30%
- **Nível de Satisfação do Cliente (CSAT)**: 3.87
- **Taxa de Transferência**: 23.10%
- **Análise de Sentimento**:
  - Positivo: 45.2%
  - Neutro: 35.6%
  - Negativo: 19.2%

### KPIs para Curadoria de Chatbot

- **Taxa de Resolução Automatizada**: 65.80%
- **Taxa de Fallback**: 12.40%
- **Tempo Médio de Resposta do Chatbot**: 2.43 segundos
- **Taxa de Engajamento**: 74.50%
- **Índice de Satisfação do Chatbot (CSAT)**: 4.12
- **Taxa de Intenções Não Reconhecidas**: 18.70%
- **Taxa de Transferência para Atendente Humano**: 15.30%

---

## Possíveis Melhorias

1. **Fonte de Dados Reais**: Conectar o script a uma fonte de dados real, como logs de chamadas e interações de chatbot, para uma análise mais precisa.
2. **Visualização**: Adicionar gráficos para visualizar os KPIs, utilizando bibliotecas como Matplotlib ou Seaborn.
3. **Análise Avançada**: Incluir análise preditiva para estimar tendências e identificar pontos de melhoria.
