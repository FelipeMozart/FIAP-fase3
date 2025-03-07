
# Plano de Teste Funcional Manual

Plano de teste funcional manual para validar o protótipo e a aplicação Glide, incluindo funcionalidades, integração com AI e experiência do usuário.


# Casos de Teste

cases:
  - name: validar-prototipo-baixa-fidelidade
    description: Validar manualmente o protótipo em baixa fidelidade (Rabiscoframe) para garantir que os fluxos principais estão claros.
    spec:
      type: manual
      steps:
        - Acessar o protótipo em baixa fidelidade.
        - Navegar pelos fluxos principais: "Iniciar um feedback", "Esclarecer uma dúvida", "Selecionar um modelo de feedback".
        - Verificar se os fluxos estão claros e funcionais.
      expected-result: Os fluxos principais devem ser compreensíveis e navegáveis.

  - name: validar-prototipo-alta-fidelidade
    description: Validar manualmente o protótipo em alta fidelidade (Figma) para verificar a interface visual e funcionalidade.
    spec:
      type: manual
      steps:
        - Acessar o protótipo em alta fidelidade no Figma.
        - Realizar as tarefas: "Iniciar um feedback", "Esclarecer uma dúvida", "Copiar um feedback sugerido pela IA", "Realizar uma busca", "Selecionar um modelo de feedback".
        - Verificar a consistência visual e funcionalidade.
      expected-result: A interface deve ser visualmente consistente e funcional.

  - name: validar-teste-usabilidade
    description: Validar manualmente o teste de usabilidade configurado no Maze com 19 participantes.
    spec:
      type: manual
      steps:
        - Revisar os resultados do teste de usabilidade no Maze.
        - Analisar as métricas: "Taxa de sucesso", "Taxa de abandono", "Taxa de erros de clique (misclicks)", "Tempo médio por tela".
        - Identificar pontos de melhoria com base nas métricas.
      expected-result: As métricas devem indicar uma experiência de usuário satisfatória.

  - name: validar-integracao-glide-openai
    description: Validar manualmente a integração entre Glide e OpenAI para geração de feedbacks estruturados.
    spec:
      type: manual
      steps:
        - Configurar a integração entre Glide e OpenAI.
        - Testar a geração de feedbacks estruturados utilizando o modelo GPT-4.
        - Verificar se os feedbacks gerados estão alinhados com o esperado.
      expected-result: A integração deve gerar feedbacks estruturados corretamente.

  - name: validar-limites-versao-free-glide
    description: Testar manualmente as limitações da versão gratuita do Glide para integração com AI e Google Sheets.
    spec:
      type: manual
      steps:
        - Configurar a versão gratuita do Glide.
        - Testar as funcionalidades: "Integração com AI", "Chamadas de API", "Uso de Google Sheets".
        - Identificar limitações e restrições.
      expected-result: As limitações da versão gratuita devem ser documentadas.

  - name: validar-implementacao-versao-business-glide
    description: Validar manualmente a implementação da versão Business do Glide para superar as limitações e garantir a funcionalidade principal do MVP.
    spec:
      type: manual
      steps:
        - Configurar a versão Business do Glide.
        - Testar as funcionalidades: "Integração nativa com AI", "Coluna Generated Column (AI)", "Componente de integração AI na interface".
        - Verificar se todas as funcionalidades estão operacionais.
      expected-result: A versão Business deve atender às necessidades do MVP sem restrições.


### **Execução dos Testes**

- **Responsável**: Equipe de construção.
- **Ferramentas**: Protótipos (Rabiscoframe, Figma), Maze, Glide (versões Free e Business), OpenAI.
- **Critérios de Aceitação**: Cada caso de teste deve atender ao resultado esperado descrito.

Este plano de teste é focado em validações manuais para garantir que as funcionalidades e a experiência do usuário estejam alinhadas com os objetivos do projeto.