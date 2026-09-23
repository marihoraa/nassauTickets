# Especificação de Requisitos - nassauTickets

## 1. Visão Geral
O sistema **nassauTickets** destina-se a gerir a emissão e o atendimento de senhas num Laboratório de Análises Clínicas, organizando a fila por prioridades e controlando os guichês de atendimento.

---

## 2. Requisitos Funcionais (RF)

| ID | Nome | Descrição |
|---|---|---|
| **RF-01** | Emissão de Senhas | O sistema deve permitir que o paciente escolha a categoria e emita uma senha (Comum ou Preferencial). |
| **RF-02** | Chamada de Senhas | O atendente deve conseguir chamar a próxima senha respeitando as regras de prioridade. |
| **RF-03** | Painel de Exibição | O sistema deve exibir na tela principal a última senha chamada e o guichê correspondente. |
| **RF-04** | Histórico Local | O sistema deve manter a lista das últimas senhas chamadas no painel. |
| **RF-05** | Finalizar Atendimento | O atendente deve alterar o status da senha para "Atendido" ou "Ausente". |

---

## 3. Requisitos Não Funcionais (RNF)

| ID | Nome | Descrição |
|---|---|---|
| **RNF-01** | Interface Web | O frontend deve ser desenvolvido utilizando **React**. |
| **RNF-02** | Usabilidade | A interface do painel deve ser legível a uma distância mínima de 3 metros. |
| **RNF-03** | Responsividade | O sistema deve funcionar adequadamente em telas de computador e monitores do painel. |
| **RNF-04** | Arquitetura | O código deve seguir a estrutura de pastas padronizada do repositório. |

---

## 4. Regras de Negócio (RN)

* **RN-01 (Prioridade):** As senhas preferenciais têm prioridade de atendimento em relação às senhas comuns (ex: proporção de 2 preferenciais para 1 comum).
* **RN-02 (Formatação da Senha):** As senhas devem conter um prefixo identificador (Ex: `P-001` para Preferencial, `C-001` para Comum).
