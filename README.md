<div align="center">

  <h1>AcadProject ICET 📚</h1>

  <p>
    <strong>Sistema Web de Gerenciamento de Projetos Acadêmicos</strong><br>
    <strong>Universidade Federal do Amazonas (UFAM) — Instituto de Ciências Exatas e Tecnologia (ICET)</sub>
  </p>

</div>

---

## 👥 Integrantes da Equipe
* **Malcon Vinicios Tavares Valente**
* **Jean Carlos Silva de Sena**

---

## 1. Introdução

### 1.1. Descrição Geral do Software
O **AcadProject ICET** é um Sistema Web de Gerenciamento de Projetos Acadêmicos focado no Instituto de Ciências Exatas e Tecnologia (ICET/UFAM). Seu objetivo é permitir que alunos e professores organizem projetos acadêmicos, distribuam tarefas, acompanhem prazos e monitorem o andamento de atividades em um único ambiente centralizado.

### 1.2. Descrição dos Usuários
Os usuários do sistema dividem-se em dois perfis principais:

* **Professores:** Usuários responsáveis pela coordenação acadêmica. Criam projetos, vinculam alunos, criam e atribuem tarefas e estipulam prazos.
* **Alunos:** Usuários participantes que visualizam os projetos aos quais estão vinculados e atualizam o status das tarefas que lhes foram atribuídas.

---

## 2. Requisitos Gerais do Software

### 2.1. Requisitos Funcionais

| ID | Descrição | Prioridade |
| :--- | :--- | :---: |
| **RF01** | O sistema deve permitir a autenticação de usuários (Login) com e-mail e senha. | Alta |
| **RF02** | O sistema deve permitir que professores criem, editem e excluam projetos acadêmicos. | Alta |
| **RF03** | O sistema deve permitir a atribuição de alunos específicos a um projeto criado. | Alta |
| **RF04** | O sistema deve permitir que tarefas sejam criadas e atribuídas a alunos com prazos definidos. | Média |
| **RF05** | O sistema deve permitir que alunos atualizem o status de suas tarefas (*A Fazer*, *Em Andamento*, *Concluído*). | Alta |
| **RF06** | O sistema deve fornecer um painel com o progresso geral e prazos pendentes. | Baixa |

### 2.2. Requisitos Não Funcionais

| ID | Descrição | Categoria |
| :--- | :--- | :---: |
| **RNF01** | O sistema deve ser acessível via navegadores web responsivos. | Usabilidade |
| **RNF02** | As senhas devem ser criptografadas no banco de dados. | Segurança |
| **RNF03** | O tempo máximo de resposta para atualização de status de tarefas deve ser inferior a 3 segundos. | Desempenho |

### 2.3. Regras de Negócio

| ID | Descrição |
| :--- | :--- |
| **RN01** | Somente usuários com perfil de "Professor" podem criar ou excluir projetos. |
| **RN02** | Um aluno só pode atualizar o status das tarefas atribuídas a ele próprio. |
| **RN03** | A data limite de uma tarefa não pode exceder a data de conclusão do projeto principal. |

---

## 3. Diagramas UML

### 3.1. Diagramas de Casos de Uso
Representa a interação dos atores **Professor** e **Aluno** com as funcionalidades do sistema AcadProject ICET (como *Criar Projeto*, *Definir Prazos*, *Atribuir Tarefa*, *Atualizar Tarefa*, *Logar*, *Recuperar Senha* e *Visualizar Projetos*).

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/aac8ba59-0d26-478c-833c-48c1a399e9bb" />


### 3.2. Diagramas de Sequência
Detalha o fluxo de mensagens do caso de uso **Criar Projeto** realizado pelo ator *Professor*, passando pelas camadas `:Interface`, `:Control` e `:Database`.

<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/2bab7897-ed4c-4de5-839f-7b88eef20d63" />


### 3.3. Diagramas de Atividades
Ilustra o fluxo de ações e validações para **Atualizar Status da Tarefa** (acessar projeto, selecionar tarefa, atualizar status, validar operação e salvar ou exibir erro).

<img width="500" height="600" alt="image" src="https://github.com/user-attachments/assets/63386914-23db-45b9-995e-7c7faaa86ad7" />
