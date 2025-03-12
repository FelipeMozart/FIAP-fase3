
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
**Execução e Resultado Alcançado**:

![](/Imagens/ct1.png)

---

**ID:** CT-02  

**Caso de Teste:** Login com código incorreto  
**Passos:**  
1. Digitar um e-mail válido.  
2. Inserir um código incorreto.  
**Resultado Esperado:** O sistema exibe uma mensagem de erro e impede o login.  
**Execução e Resultado Alcançado**:

![](/Imagens/ct2.png)


---


**ID:** CT-03 

**Caso de Teste:** Criar um feedback válido  
**Passos:**  
1. Acessar a tela de "Novo Feedback".  
2. Preencher os campos obrigatórios.  
3. Clicar em "Assistente AI"; 
4. Visualizar feedback final gerado; 
5. Editar se necessário e salvar.  
**Resultado Esperado:** O feedback é salvo corretamente e aparece na lista.  
**Execução e Resultado Alcançado**:

![](/Imagens/ct3.png)

---

**ID:** CT-04

**Caso de Teste:** Verificar se feedbacks aparecem apenas para quem criou  
**Passos:**  
1. Criar um feedback com um usuário.  
2. Logar com outro usuário.  
3. Acessar a lista de feedbacks.  
**Resultado Esperado:** O segundo usuário não vê feedbacks criados por outros usuários.

**Execução e Resultado Alcançado**:


![](/Imagens/ct4.png)


---

**ID:** CT-05

**Caso de Teste:** Editar um feedback existente  
**Passos:**  
1. Acessar a tela de feedbacks.  
2. Selecionar um feedback criado.  
3. Editar o texto.  
4. Salvar as alterações.  
**Resultado Esperado:** O feedback é atualizado corretamente no banco.  
**Execução e Resultado Alcançado**:

![](/Imagens/ct5.png)

---

**ID:** CT-06

**Caso de Teste:** Criar um chamado válido  
**Passos:**  
1. Acessar a tela de suporte.  
2. Preencher os campos obrigatórios.  
3. Clicar em "Enviar".  
**Resultado Esperado:** O chamado é salvo corretamente e aparece a mensagem de sucesso.  
**Execução e Resultado Alcançado**:

![](/Imagens/ct6.png)

---

**ID:** CT-07 

**Caso de Teste:** Criar um chamado sem descrição  
**Passos:**  
1. Acessar a tela de suporte.  
2. Deixar o campo de descrição em branco.  
3. Tentar salvar.  
**Resultado Esperado:** O sistema não deve permitir clicar no botão "Enviar". 
**Execução e Resultado Alcançado**:

![](/Imagens/ct7.png)


---
**ID:** CT-08

**Caso de Teste:** Alterar perfil de usuário. 
**Passos:**  
1. Navegar até a home.  
2. Clicar no email de usuário e, depois, em "Ver perfil".  
3. Preencher os campos necessários.  
4. Clicar em "Enviar".
**Resultado Esperado:** O sistema deve registrar as atualizações.  
**Execução e Resultado Alcançado**:

![](/Imagens/ct8.png)

---
**ID:** CT-09

**Caso de Teste:** Buscar perfil de usuário. 
**Passos:**  
1. Navegar até a home.  
2. No campo de pesquisa busque por um usuário válido.  
**Resultado Esperado:** O sistema deve retornar todos os registros de um usuário válido.  
**Execução e Resultado Alcançado**:

![](/Imagens/ct9.png)


---
**ID:** CT-10

**Caso de Teste:** Buscar perfil de usuário e filtrar por um ciclo específico. 
**Passos:**  
1. Navegar até a home.  
2. No campo de pesquisa busque por um usuário válido. 
3. Aplicar filtro para retornar apenas apenas um ciclo.
**Resultado Esperado:** O sistema deve retornar o registro de um usuário válido.  
**Execução e Resultado Alcançado**:

![](/Imagens/ct10.png)

---

**ID:** CT-11

**Caso de Teste:** Teste de múltiplos usuários acessando simultaneamente  
**Passos:**  
1. Criar 5 usuários de teste.  
2. Cada usuário cria um feedback simultaneamente.  
3. Verificar se há travamentos ou inconsistências.  
**Resultado Esperado:** O sistema deve continuar funcionando sem erro ou lentidão.


**Execução e Resultado Alcançado**:

Horário de Início: 10:22
Quantidade de Usuários: 6
Quantidade de Feedbacks Registrados: 50
Quantidade de Chamados Registrados: 30
Distribuição de Usuários e Feedbacks Criados:
- Andre: SUELI, ALICE e LAZARO;
- Felipe: OTAVIO, GUILHERME e MARIA;
- Douglas: ANGELITA, LAZARA e JOAO.

Navegadores utilizados:
- Google Chrome
- Microsoft Edge
- Safari

Observações: o sistema manteve a estabilidade durante o teste, sem apresentar travamentos ou inconsistências.