
# Plano de Teste Funcional Manual

Plano de teste funcional manual para validar o protótipo e a aplicação Glide, incluindo funcionalidades, integração com AI e experiência do usuário.


## Casos de Teste


### Caso 1: Validar Protótipo em Baixa Fidelidade
- **Nome**: validar-prototipo-baixa-fidelidade
- **Descrição**: Validar manualmente o protótipo em baixa fidelidade (Rabiscoframe) para garantir que os fluxos principais estão claros.
- **Especificação**:
  - **Tipo**: manual
  - **Passos**:
    1. Acessar o protótipo em baixa fidelidade.
    2. Navegar pelos fluxos principais: "Iniciar um feedback", "Esclarecer uma dúvida", "Selecionar um modelo de feedback".
    3. Verificar se os fluxos estão claros e funcionais.
  - **Resultado Esperado**: Os fluxos principais devem ser compreensíveis e navegáveis.

---

### Caso 2: Validar Protótipo em Alta Fidelidade
- **Nome**: validar-prototipo-alta-fidelidade
- **Descrição**: Validar manualmente o protótipo em alta fidelidade (Figma) para verificar a interface visual e funcionalidade.
- **Especificação**:
  - **Tipo**: manual
  - **Passos**:
    1. Acessar o protótipo em alta fidelidade no Figma.
    2. Realizar as tarefas: "Iniciar um feedback", "Esclarecer uma dúvida", "Copiar um feedback sugerido pela IA", "Realizar uma busca", "Selecionar um modelo de feedback".
    3. Verificar a consistência visual e funcionalidade.
  - **Resultado Esperado**: A interface deve ser visualmente consistente e funcional.

---

### Caso 3: Validar Teste de Usabilidade
- **Nome**: validar-teste-usabilidade
- **Descrição**: Validar manualmente o teste de usabilidade configurado no Maze com 19 participantes.
- **Especificação**:
  - **Tipo**: manual
  - **Passos**:
    1. Revisar os resultados do teste de usabilidade no Maze.
    2. Analisar as métricas: "Taxa de sucesso", "Taxa de abandono", "Taxa de erros de clique (misclicks)", "Tempo médio por tela".
    3. Identificar pontos de melhoria com base nas métricas.
  - **Resultado Esperado**: As métricas devem indicar uma experiência de usuário satisfatória.

---

### Caso 4: Validar Integração Glide e OpenAI
- **Nome**: validar-integracao-glide-openai
- **Descrição**: Validar manualmente a integração entre Glide e OpenAI para geração de feedbacks estruturados.
- **Especificação**:
  - **Tipo**: manual
  - **Passos**:
    1. Configurar a integração entre Glide e OpenAI.
    2. Testar a geração de feedbacks estruturados utilizando o modelo GPT-4.
    3. Verificar se os feedbacks gerados estão alinhados com o esperado.
  - **Resultado Esperado**: A integração deve gerar feedbacks estruturados corretamente.

---

### Caso 5: Validar Limites da Versão Free do Glide
- **Nome**: validar-limites-versao-free-glide
- **Descrição**: Testar manualmente as limitações da versão gratuita do Glide para integração com AI e Google Sheets.
- **Especificação**:
  - **Tipo**: manual
  - **Passos**:
    1. Configurar a versão gratuita do Glide.
    2. Testar as funcionalidades: "Integração com AI", "Chamadas de API", "Uso de Google Sheets".
    3. Identificar limitações e restrições.
  - **Resultado Esperado**: As limitações da versão gratuita devem ser documentadas.

---

### Caso 6: Validar Implementação da Versão Business do Glide
- **Nome**: validar-implementacao-versao-business-glide
- **Descrição**: Validar manualmente a implementação da versão Business do Glide para superar as limitações e garantir a funcionalidade principal do MVP.
- **Especificação**:
  - **Tipo**: manual
  - **Passos**:
    1. Configurar a versão Business do Glide.
    2. Testar as funcionalidades: "Integração nativa com AI", "Coluna Generated Column (AI)", "Componente de integração AI na interface".
    3. Verificar se todas as funcionalidades estão operacionais.
  - **Resultado Esperado**: A versão Business deve atender às necessidades do MVP sem restrições.


### **Execução dos Testes**

- **Responsável**: Equipe de construção.
- **Ferramentas**: Protótipos (Rabiscoframe, Figma), Maze, Glide (versões Free e Business), OpenAI.
- **Critérios de Aceitação**: Cada caso de teste deve atender ao resultado esperado descrito.

Este plano de teste é focado em validações manuais para garantir que as funcionalidades e a experiência do usuário estejam alinhadas com os objetivos do projeto.