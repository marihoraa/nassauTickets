# nassauTickets

Sistema de Controle de Atendimento para um Laboratório de Análises Clínicas.

## Descrição

O nassauTickets é um sistema de controle de atendimento desenvolvido para um Laboratório de Análises Clínicas. Ele gerencia a emissão, fila, chamada e atendimento de senhas, contemplando três tipos de senha (Prioritária, Geral e para Retirada de Exames) e regras de priorização, painel de chamadas, relatórios e auditoria, conforme os requisitos e regras de negócio definidos na documentação do projeto.

## Objetivo

Esta atividade tem como objetivo consolidar os conhecimentos de desenvolvimento Web, organização de projetos, Git/GitHub, documentação, React e integração entre as partes de uma aplicação, através do desenvolvimento em grupo de um sistema completo, versionado e documentado.

## Tecnologias utilizadas

- **Frontend:** React 19
- **Backend:** *a definir pelo grupo (Node.js LTS 22 com Express, Java 21 com Spring Boot ou Python 3.14 com Flask/FastAPI)*
- **Banco de dados:** MySQL 8.0

*Assim que o grupo definir a tecnologia de backend, esta seção será atualizada com a justificativa da escolha.*

## Arquitetura / Visão geral

O sistema trabalha com três agentes principais:

- **AS (Agente Sistema):** executa as ações do sistema, comunica-se com o banco de dados e demais infraestruturas, emite senhas, atualiza o painel e responde aos comandos dos demais agentes.
- **AA (Agente Atendente):** responsável por chamar o próximo cliente e realizar o atendimento no guichê.
- **AC (Agente Cliente):** emite sua senha por meio do totem e aguarda a chamada no painel.

## Instalação e execução

### Frontend

```
cd frontend
npm install
npm run dev
```

### Backend

*Instruções de instalação e execução serão adicionadas assim que a tecnologia de backend for definida pelo grupo.*

## Configuração

*Informações sobre variáveis de ambiente e configuração do banco de dados serão adicionadas quando o backend for implementado.*

## Membros

| Nome | Matrícula | Papel|
|-------------------------------|-----------|----------|
| Maria Eduarda Cavalcante Hora | 01603709  | Scrum Master  |
| Tereza Ana Barros e Silva | 01830940  | Documentador  |
| Giovanna Cavalcanti Melo  | 01828278  | Documentador  |
| Anna Julia Seixas Silva   | 01755954  | Desenvolvedor |
| Diogenes Raimundo Da Silva | 01777145 | Desenvolvedor |
| Laura Marques de Arandas  | 01850581  | Testador      |

### Papéis dos membros

- **Scrum Master:** responsável pela criação e organização do repositório e pela coordenação das atividades relacionadas ao projeto.
- **Documentador:** responsável pela produção e organização da documentação (requisitos, MER, mockups, diagramas UML).
- **Desenvolvedor:** responsável pela implementação e evolução do código (frontend e backend).
- **Testador:** responsável pela verificação do funcionamento, identificação de problemas e validação das funcionalidades.

## Branches

- **main:** versões estáveis e revisadas do projeto.
- **dev:** branch de desenvolvimento, onde o time trabalha no dia a dia. Todo o código é enviado primeiro para a `dev` e, posteriormente, integrado à `main` por meio de merge.

## Estrutura do repositório

```
nassauTickets/
├── backend/
├── docs/
│   ├── branding/
│   ├── mer/
│   ├── mockups/
│   ├── models/
│   │   └── uml/
│   └── requirements/
├── frontend/
├── .gitignore
├── LICENSE
└── README.md
```

## Licença

Este projeto está licenciado sob a licença MIT — veja o arquivo [LICENSE](LICENSE) para mais detalhes.
