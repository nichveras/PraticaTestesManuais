## 🧪 **Plano de Testes - OrangeHRM (Demo)**

### 📌 1. **Identificação**

* **Nome do Projeto**: OrangeHRM - Sistema de Gestão de Recursos Humanos
* **Versão Avaliada**: Demo pública
* **Ambiente de Testes**: [https://opensource-demo.orangehrmlive.com](https://opensource-demo.orangehrmlive.com)
* **Tipo de Teste**: Teste Funcional Manual
* **Data do Documento**: 17/05/2026
* **Responsável**: Nicholas Veras

---

### 🎯 2. **Objetivo**

Realizar a verificação manual dos principais requisitos funcionais do sistema OrangeHRM Demo com foco em validação dos fluxos críticos, mensagens de erro, comportamento esperado e integridade das funcionalidades disponíveis na interface web.

---

### 🧩 3. **Escopo**

**Incluído:**

* Autenticação de usuário
* Dashboard inicial
* Gestão de funcionários (PIM)
* Férias (Leave)
* Recrutamento
* Administração (Admin)
* Controle de ponto (Time)
* Diretório e relatórios

**Excluído:**

* Testes de integração com sistemas externos (não disponíveis na demo)
* Testes em dispositivos móveis
* Testes de performance ou carga

---

### 🔧 4. **Ferramentas Utilizadas**

* Navegador Google Chrome / Firefox
* Ferramentas de inspeção do navegador (DevTools)
* Google Sheets, Excel ou Sistema próprio de gerenciamento de testes (registro de casos e evidências)
* Captura de tela (Jam.dev)

---

### 🧪 5. **Técnicas de Teste**

* Particionamento de equivalência
* Análise de valor limite
* Caminho feliz (Happy Path)
* Testes negativos
* Testes exploratórios

---

### 📄 6. **Critérios de Aceitação**

* Todos os casos de teste devem passar com sucesso, conforme o resultado esperado.
* Nenhuma falha crítica deve estar presente em funcionalidades principais.
* Mensagens de erro e validações devem ser consistentes.

---

### 🚦 7. **Critérios de Saída (Exit Criteria)**

* Todos os testes do escopo foram executados.
* Falhas foram registradas, analisadas e reexecutadas se necessário.
* Documentação de evidências de sucesso e falhas está completa.

---

### ⏱️ 8. **Cronograma Estimado**

| Atividade                   | Data Início | Data Fim   |
| --------------------------- | ----------- | ---------- |
| Planejamento de Testes      | 17/05/2026  | 17/05/2026 |
| Criação de Casos de Teste   | 17/05/2026  | 17/05/2026 |
| Execução dos Testes Manuais | 17/05/2026  | 17/05/2026 |
| Registro e Report de Bugs   | 17/05/2026  | 17/05/2026 |
| Encerramento e Evidências   | 17/05/2026  | 17/05/2026 |

---

### 📋 9. **Módulos a Serem Testados**

| Código RF | Módulo                   | Prioridade |
| --------- | ------------------------ | ---------- |
| RF01      | Login                    | Alta       |
| RF02      | Dashboard                | Média      |
| RF03      | PIM - Funcionários       | Alta       |
| RF04      | Férias (Leave)           | Alta       |
| RF05      | Recrutamento             | Média      |
| RF06      | Administração (Admin)    | Alta       |
| RF07      | Controle de Ponto (Time) | Média      |
| RF08      | Relatórios               | Média      |
| RF09      | Diretório                | Baixa      |
| RF10      | Manutenção               | Baixa      |

---

### 🐞 10. **Gestão de Defeitos**

* Bugs serão documentados com:

  * Título
  * Descrição
  * Passos para reproduzir
  * Evidência (print ou vídeo)
  * Gravidade (Crítica, Alta, Média, Baixa)
* Ferramenta sugerida: Google Sheets ou Jira (para simulação)

---

### 📌 11. **Riscos Identificados**

| Risco                                  | Impacto | Mitigação                        |
| -------------------------------------- | ------- | -------------------------------- |
| Sistema fora do ar                     | Alto    | Tentar novamente após intervalo  |
| Dados da demo não sendo persistentes   | Médio   | Refazer cenários se necessário   |
| Testes limitados à conta "Admin" única | Médio   | Documentar esse limite no escopo |

---

### 📁 12. **Entregáveis**

* Plano de Testes (.md ou .pdf)
* Casos de Teste (.md ou planilha)
* Evidências de Execução (prints organizados por RF)
* Registro de Bugs (se houver)
* Relatório Final de Execução
