# Projeto Chatbot Dra. Jô

## Escopo do Projeto
O chatbot **Dra. Jô** foi projetado para atender todas as necessidades de comunicação virtual de uma empresa, onde os dados necessários para essa troca de informações sejam acessíveis online, necessitando apenas da integração com as informações e a definição de um fluxo. O sistema pode ser utilizado para atendimento ao cliente, agendamentos, vendas, suporte técnico, entre outras opções.

## Tipo de Chatbot
- **Baseado em IA/NLP** orientado a uma lista pré-programada de funções e contextos.

## Camadas de Arquitetura
1. **Banco de Dados**
   - **Plataforma:** Azure Database for MySQL
   - **Banco de Dados:** MySQL
   - **Custo:** Inicia em USD$15

2. **Inteligência Artificial**
   - **Plataforma:** OpenAI
   - **Modelo:** gpt-4o-mini
   - **Custo:** 1 Milhão de tokens (~750 mil palavras)
     - **Leitura:** USD$0.150 / 1M tokens
     - **Armazenamento (cache):** USD$0.075 / 1M tokens
     - **Resposta:** USD$0.600 / 1M tokens

3. **Back-End**
   - **Plataforma:** Azure App Service
   - **Linguagem:** Python
   - **Custo:** Inicia em USD$13

4. **Front-End**
   - **Plataforma:** Twilio
   - **Sistema:** WhatsApp
   - **Custo:** USD$0.005 por mensagem

## Boas Práticas
Devido à sensibilidade de informações referentes ao usuário ou empresa, para alguns tipos de dados deve ser solicitada autenticação via e-mail ou SMS previamente cadastrados.

## Tecnologias
- Python, RESTful APIs, MySQL

## Descrição dos Elementos
- **Front-End:** O WhatsApp permite que o usuário se conecte com o sistema para enviar perguntas e arquivos, recebendo respostas de acordo com o fluxo definido.
- **Back-End:** O sistema, desenvolvido em Python, orienta as decisões da inteligência artificial, conectando as informações disponíveis online com o usuário, sejam elas informações didáticas ou concretas, como uma nota fiscal ou um boleto. Também permite o cadastro de novos fluxos, editando o comportamento do chatbot em tempo real.
- **Banco de Dados:** Armazena as regras dos fluxos de conversas e os históricos para consultas futuras, permitindo que o sistema se lembre de conversas anteriores e mantenha o contexto completo.
- **Inteligência Artificial:** O modelo de linguagem natural humaniza, interpreta e decide, adaptando o chatbot para diferentes tipos de conversas, desde formais a informais.

## Custo por Camada
- **Banco de Dados:** Inicia em USD$15
- **Inteligência Artificial:** 
  - **Leitura:** USD$0.150 / 1M tokens
  - **Armazenamento (cache):** USD$0.075 / 1M tokens
  - **Resposta:** USD$0.600 / 1M tokens
- **Back-End:** Inicia em USD$13
- **Front-End:** USD$0.005 por mensagem

## Resultados Esperados
O sistema ajudará a reduzir tempos de espera e aumentar a satisfação do cliente, permitindo que a equipe se concentre em atividades de maior valor agregado, como desenvolvimento de estratégias e inovação.

### Valores Agregados ao Modelo de Negócio
- **Automação e Escalabilidade:** Lida com grandes volumes de consultas simultâneas.
- **Aprimoramento do Atendimento ao Cliente:** Respostas rápidas e precisas melhoram a experiência do cliente.
- **Redução de Custos Operacionais:** Menor necessidade de ampliar a equipe de suporte.
- **Captação de Dados e Insights:** Coleta dados sobre interações que revelam tendências para otimizar o atendimento e produtos.

### Ganhos e Possíveis Perdas
- **Ganhos:**
  - **Eficiência Operacional:** Respostas automáticas e ágeis.
  - **Fidelização do Cliente:** Atendimento personalizado pode aumentar a retenção.
  - **Economia de Recursos:** Reduz a necessidade de mão de obra para tarefas rotineiras.
- **Possíveis Perdas:**
  - **Custos Iniciais e de Manutenção:** Apesar da economia a longo prazo, há um investimento inicial e custos recorrentes.

