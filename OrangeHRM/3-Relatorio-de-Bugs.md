# Relatório de Bugs

**Software:** OrangeHRM

**QA responsável:** Nicholas Veras

**Data:** 17.05.26

---

### 🐞 **Bug 01: Ícone de visualizar senha não existe**

| **ID**     | **Descrição**                                                                                                                                             |
| ---------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BUG-001    | O ícone de “ver senha” não existe, impedindo o usuário de visualizar a senha digitada. |

| **Severidade do Bug** | **Prioridade de Correção** | **Status** |
| :-------------------: | :------------------------: | :--------: |
|         Média         |            Alta            |   Aberto   |

| **Passo a passo para simular o bug**                           |
| -------------------------------------------------------------- |
| 1. Acessar a página de login                                   |
| 2. Digitar a senha no campo apropriado                         | |

|                        **Comportamento Esperado**                       |                        **Comportamento Obtido**                        |
| :---------------------------------------------------------------------: | :--------------------------------------------------------------------: |
| O ícone de "ver senha" deve ser visível. | impede o usuário de visualizar a senha e verificar se está correta. |

| **Ambiente**             |
| ------------------------ |
| Ambiente de homologação. |
| Linux (x86).             |
| Cromo 147.0.7727.116     |
| OrangeHRM Demo           |

| **Funcionalidade Afetada** |        **Caso de Teste Relacionado**       |
| :------------------------: | :----------------------------------------: |
| Login / Criação de usuário | C01-CT01: Login com e-mail e senha válidos |

|                **Evidência(s)**               |
| :-------------------------------------------: |
| [Vídeo](https://jam.dev/c/d7afae32-eb41-401c-82c2-d26fb99ede89) |

---
#### Bug 02: Página de login atualiza ao ocorrer erro de autenticação

| **ID**     | **Descrição**                                                                                                          |
| ---------- | ------------------------------------------------------------------------------------------------------------------------ |
| BUG-002    | Ao inserir credenciais incorretas no login, a página é atualizada, o que prejudica a experiência do usuário (UX/UI).    |

| **Severidade do Bug** | **Prioridade de Correção** | **Status** |
| :-------------------: | :------------------------: | :--------: |
|         Baixa         |           Média            |   Aberto   |

| **Passo a passo para simular o bug**                        |
| ----------------------------------------------------------- |
| 1. Acessar a página de login                                |
| 2. Inserir um nome de usuário ou senha inválidos            |
| 3. Clicar no botão "Login"                                  |

|                     **Comportamento Esperado**                      |                   **Comportamento Obtido**                   |
| :-----------------------------------------------------------------: | :-----------------------------------------------------------: |
| Exibir mensagem de erro sem atualizar a página                     | A página é atualizada e apenas então exibe a mensagem de erro |

| **Ambiente**             |
| ------------------------ |
| Ambiente de homologação. |
| Linux (x86).             |
| Cromo 147.0.7727.116     |
| OrangeHRM Demo           |

| **Funcionalidade Afetada** |         **Caso de Teste Relacionado**         |
| :------------------------: | :-------------------------------------------: |
|           Login            | C01-CT02: Login com credenciais inválidas     |

|              **Evidência(s)**              |
| :----------------------------------------: |
| [Vídeo](https://jam.dev/c/c6faa0bf-605d-4d6b-9f0f-7136ecb75522) |

---
#### Bug 03: Não há mensagem clara de sucesso ou falha no login

| **ID**     | **Descrição**                                                                                                     |
| ---------- | ------------------------------------------------------------------------------------------------------------------- |
| BUG-003    | O sistema não exibe mensagens de sucesso ou erro de forma clara após login, apenas redireciona ou atualiza a página. |

| **Severidade do Bug** | **Prioridade de Correção** | **Status** |
| :-------------------: | :------------------------: | :--------: |
|         Média          |           Média            |   Aberto   |

| **Passo a passo para simular o bug**              |
| ------------------------------------------------- |
| 1. Acessar a página de login                      |
| 2. Inserir credenciais válidas                    |
| 3. Clicar em "Login"                              |

|                   **Comportamento Esperado**                   |                 **Comportamento Obtido**                  |
| :-------------------------------------------------------------: | :--------------------------------------------------------: |
| Mensagem como "Login realizado com sucesso" deve ser exibida   | Usuário é redirecionado diretamente sem mensagem alguma    |

| **Ambiente**             |
| ------------------------ |
| Ambiente de homologação. |
| Linux (x86).             |
| Cromo 147.0.7727.116     |
| OrangeHRM Demo           |

| **Funcionalidade Afetada** |         **Caso de Teste Relacionado**         |
| :------------------------: | :-------------------------------------------: |
|           Login            | C01-CT01: Login com e-mail e senha válidos    |

|               **Evidência(s)**               |
| :------------------------------------------: |
| [Vídeo](https://jam.dev/c/4146d59c-ee23-4b4f-866c-3f1af478f0b3)  |

---
#### Bug 04: Não é possível aplicar licença de férias - "No Leave Types with Leave Balance"

| **ID**     | **Descrição**                                                                                                                |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------ |
| BUG-004    | Ao tentar aplicar uma licença no módulo de férias, nenhuma opção de licença é exibida, impossibilitando a solicitação.        |

| **Severidade do Bug** | **Prioridade de Correção** | **Status** |
| :-------------------: | :------------------------: | :--------: |
|        Alta            |           Alta             |   Aberto   |

| **Passo a passo para simular o bug**                     |
| -------------------------------------------------------- |
| 1. Acessar o menu "Leave"                                |
| 2. Clicar em "Apply"                                     |
| 3. Verificar se aparecem tipos de licença disponíveis    |

|                      **Comportamento Esperado**                       |                        **Comportamento Obtido**                         |
| :-------------------------------------------------------------------: | :----------------------------------------------------------------------: |
| Deve-se exibir uma lista de tipos de licença com saldo disponível     | A mensagem "No Leave Types with Leave Balance" é exibida e nada é listado |

| **Ambiente**             |
| ------------------------ |
| Ambiente de homologação. |
| Linux (x86).             |
| Cromo 147.0.7727.116     |
| OrangeHRM Demo           |

| **Funcionalidade Afetada** |               **Caso de Teste Relacionado**               |
| :------------------------: | :-------------------------------------------------------: |
|    Férias (Leave Module)   | C04-CT01: Aplicar licença de férias com dados válidos     |

|              **Evidência(s)**              |
| :----------------------------------------: |
| [Vídeo](https://jam.dev/c/d4802406-7a6f-4031-a63a-457c6dddfcf4) |

---
#### Bug 05: Ícone de “ver senha” não existe no formulário de criação de funcionário

| **ID**     | **Descrição**                                                                                                                                                  |
| ---------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BUG-005    | No formulário de criação de funcionário no módulo PIM, o ícone de "ver senha" não existe.             |

| **Severidade do Bug** | **Prioridade de Correção** | **Status** |
| :-------------------: | :------------------------: | :--------: |
|         Média         |           Alta             |   Aberto   |

| **Passo a passo para simular o bug**                             |
| ---------------------------------------------------------------- |
| 1. Navegar até o módulo "PIM"                                    |
| 2. Clicar em "Add Employee"                                      |
| 3. Marcar a opção "Create Login Details"                         |
| 4. Observar o campo de senha se há o ícone de "ver senha"        |


|                      **Comportamento Esperado**                      |                         **Comportamento Obtido**                          |
| :------------------------------------------------------------------: | :------------------------------------------------------------------------: |
| O ícone de "ver senha" deve ser visível e funcional, impedindo visualização |

| **Ambiente**             |
| ------------------------ |
| Ambiente de homologação. |
| Linux (x86).             |
| Cromo 147.0.7727.116     |
| OrangeHRM Demo           |

| **Funcionalidade Afetada** |            **Caso de Teste Relacionado**             |
| :------------------------: | :--------------------------------------------------: |
| Cadastro de funcionário    | C03-CT01: Criar novo funcionário com dados válidos   |

|               **Evidência(s)**               |
| :------------------------------------------: |
| [Vídeo](mesmo bug do 001) |

---

   |
