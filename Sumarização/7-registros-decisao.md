# Tomada de Decisão

## Informações do Projeto - Protótipo

Para garantir a validação das ideias e a eficiência no desenvolvimento do produto, foram definidas as seguintes diretrizes para o protótipo:

- **Protótipo em baixa fidelidade**: Rabiscoframe, para esboçar rapidamente as ideias iniciais;
- **Protótipo em alta fidelidade**: Figma, para criar uma interface visualmente rica e funcional;
- **Plataforma para teste de usabilidade**: Maze, para coletar feedbacks e avaliar a experiência do usuário;
- **Amostra necessária**: 15 respostas, garantindo uma base mínima para análise;
- **Forma de captação**: envio do link para os participantes selecionados.

###  Etapas

As etapas para a construção e validação do protótipo foram organizadas da seguinte forma:

1. **Ideia geral no papel**: esboço inicial das funcionalidades e fluxos principais;
2. **Desenvolvimento da primeira versão no Figma**: criação de um protótipo visual e interativo;
3. **Simplificação da interface**: ajustes para aproximar o design das possibilidades de desenvolvimento no Glide para o MVP;
4. **Formatação do teste no Maze**: configuração do teste de usabilidade e início do envio para os participantes.


## Informações do projeto - Aplicação Glide

### Decisões Tomadas

- **Assinatura do Glide Business**: contratado por U$ 249,00 mensais. Cancelamento necessário até o dia **10/03/2025**;
- **Assinatura da OpenAI API**: Plataforma **platform.openai.com** com crédito inicial de **U$ 5,00**.

### Arquitetura e Tecnologias

- **Glide Apps**: Utilização de tecnologia NoCode para desenvolvimento rápido e eficiente;
- **Banco de Dados**: Glide Tables, integrado diretamente à aplicação;
- **AI Utilizada**: OpenAI;
  - **Modelo ChatGPT**: gpt-4;
  - **Prompt**: "Esse é um rascunho de um feedback, com base no texto, me sugira um feedback estruturado, destacando pontos fortes, pontos de desenvolvimento e próximos passos."

### Desafios Tecnológicos

#### Integração Glide com AI

- **Limitações da Versão Free**:
  
  - A versão gratuita do Glide não oferece suporte para integrações, chamadas de APIs e uso de Google Sheets;
  - A ausência de suporte ao Google Sheets inviabilizou a alternativa de usar Google Sheets, Apps Script e Pipedream (webhook) para contornar as limitações. O fluxo planejado seria:
    1. Glide chamaria o Pipedream;
    2. Pipedream faria um POST no Google Sheets (aba entrada);
    3. Google Sheets acionaria o Apps Script;
    4. Apps Script faria POST e GET na API OpenAI;
    5. Apps Script pegaria o retorno e salvaria no Google Sheets (aba saída);
    6. Google Sheets chamaria o Pipedream;
    7. Pipedream retornaria para o Glide.
  - Devido a essas restrições, a versão gratuita do Glide não atendeu às necessidades do projeto.

- **Solução Adotada**:
  
  - Optamos por assinar a versão **Business** do Glide para superar as limitações e garantir a funcionalidade principal do MVP: integração e interação nativa com AI;
  - Durante o período de trial (30 dias), conseguimos implementar e validar a solução.

#### Implementação na Versão Business

- **Integração AI**:
  
  - Utilizamos duas opções de integração com AI:
    1. **Banco de Dados**: coluna do tipo **Generated Column (AI)**;
    2. **Interface**: componente com ação de integração AI diretamente na interface do Glide.