
# Plano de Teste

O plano de testes da aplicação Glide foi elaborado com o objetivo de garantir a qualidade e o correto funcionamento das principais funcionalidades do sistema.

Este documento descreve uma série de casos de teste que cobrem diversos cenários, como login  de usuários, criação e gerenciamento de feedbacks, abertura de chamados e testes de desempenho com múltiplos usuários. 

Cada caso de teste inclui passos detalhados e o resultado esperado, permitindo uma validação clara e objetiva do comportamento do sistema. A execução desses testes é necessária para identificar possíveis falhas e assegurar que a aplicação atenda aos requisitos funcionais esperados pelos usuários.


**ID:** CT-01  

**Caso de Teste:** Login com e-mail válido  
**Passos:**  
1. Acessar a tela de login.  
2. Digitar e-mail válido.  
3. Receber código no e-mail.  
4. Inserir código corretamente.  
5. Acessar a aplicação.  
**Resultado Esperado:** O usuário é autenticado e acessa o sistema.  

---

**ID:** CT-02  

**Caso de Teste:** Login com código incorreto  
**Passos:**  
1. Digitar um e-mail válido.  
2. Inserir um código incorreto.  
**Resultado Esperado:** O sistema exibe uma mensagem de erro e impede o login.  

---


**ID:** CT-03 

**Caso de Teste:** Criar um feedback válido  
**Passos:**  
1. Acessar a tela de "Novo Feedback".  
2. Preencher os campos obrigatórios.  
3. Clicar em "Gerar Feedback".  
4. Visualizar feedback gerado.  
5. Editar se necessário e salvar.  
**Resultado Esperado:** O feedback é salvo corretamente e aparece na lista.  

---

**ID:** CT-04

**Caso de Teste:** Verificar se feedbacks aparecem apenas para quem criou  
**Passos:**  
1. Criar um feedback com um usuário.  
2. Logar com outro usuário.  
3. Acessar a lista de feedbacks.  
**Resultado Esperado:** O segundo usuário não vê feedbacks criados por outros usuários.  

---

**ID:** CT-05

**Caso de Teste:** Editar um feedback existente  
**Passos:**  
1. Acessar a tela de feedbacks.  
2. Selecionar um feedback criado.  
3. Editar o texto.  
4. Salvar as alterações.  
**Resultado Esperado:** O feedback é atualizado corretamente no banco.  

---

**ID:** CT-06

**Caso de Teste:** Criar um chamado válido  
**Passos:**  
1. Acessar a tela de suporte.  
2. Preencher motivo e descrição.  
3. Clicar em "Abrir Chamado".  
**Resultado Esperado:** O chamado é salvo corretamente e aparece na lista do usuário.  

---

**ID:** CT-07 

**Caso de Teste:** Criar um chamado sem descrição  
**Passos:**  
1. Acessar a tela de suporte.  
2. Deixar o campo de descrição em branco.  
3. Tentar salvar.  
**Resultado Esperado:** O sistema exibe uma mensagem de erro impedindo o salvamento.  

---

**ID:** CT-08

**Caso de Teste:** Teste de múltiplos usuários acessando simultaneamente  
**Passos:**  
1. Criar 5 usuários de teste.  
2. Cada usuário cria um feedback simultaneamente.  
3. Verificar se há travamentos ou inconsistências.  
**Resultado Esperado:** O sistema deve continuar funcionando sem erro ou lentidão.  