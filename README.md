# FuteVôlei Hub — MVP
 
## Resumo do projeto
 
App Android para gamificação de arenas de futevôlei, desenvolvido como parte do programa de pós-graduação em Engenharia de Software da PUC-Rio.
 
O MVP foca na jornada do jogador Gabriel — criando desafios em dupla com produtos reais da arena como recompensa e resgatando os prêmios após a vitória.
 
---
 
## 1. O problema e o contexto
 
Jogadores de futevôlei não têm uma forma estruturada de se desafiar entre si, registrar resultados e ganhar recompensas dentro da sua arena. Os desafios são combinados informalmente, os resultados não são registrados e não há nenhum mecanismo de engajamento entre as aulas.
 
O FuteVôlei Hub resolve esse problema com um app Android onde jogadores criam desafios em dupla, apostam produtos reais da loja da arena e resgatam suas recompensas após a vitória — tornando cada treino uma experiência competitiva e motivadora.
 
---
 
## 2. O workshop de Lean Inception
 
Uma Lean Inception completa foi conduzida no Miro, cobrindo todas as 9 etapas da metodologia:
 
- **Kickoff** — alinhamento do time e apresentação dos stakeholders
- **Etapa 1 — Visão do Produto** — proposta de valor definida para jogadores de arenas de futevôlei
- **Etapa 2 — É / Não É / Faz / Não Faz** — o app gamifica desafios entre jogadores; não substitui o professor nem gerencia a arena operacionalmente
- **Etapa 3 — Objetivos do Negócio** — aumentar o engajamento dos alunos, diferenciar a arena pela gamificação e construir um produto B2B escalável
- **Etapa 4 — Personas** — Gabriel (aluno, 36 anos)
- **Etapa 5 — Jornadas do Usuário** — 1 jornadas mapeada: desafiar um jogador, acompanhar o ranking e resgatar uma recompensa
- **Etapa 6 — Brainstorming de Funcionalidades** — funcionalidades identificadas a partir das jornadas e classificadas por esforço, valor de negócio e valor de UX
- **Etapa 7 — Revisão Técnica, de UX e de Negócio** — funcionalidades avaliadas com escala EEE/$$$/♥♥♥
- **Etapa 8 — Sequenciador** — ondas do MVP + ondas de incremento definidas
- **Etapa 9 — MVP Canvas** — MVP sintetizado com proposta, personas, jornadas, funcionalidades, métricas e custo
---
 
## 3. Arquitetura do produto
 
```
[MVP — Sprint 1]                               [Incrementos]
Perfil do jogador (lado + nível)    ══════>    Incremento 1: Ranking
Desafios em dupla com recompensa               Métricas individuais por jogador
Aceitar e recusar desafios                     histórico de partidas por jogador
Registrar resultado                            
Resgatar recompensa pelo app                   
Cancelar desafio                                             
```
 
- **Sprint 1 — MVP** — jornada completa do jogador: perfil, desafios em dupla e resgate de recompensa
- **Sprint 2 — Incremento 1** — ranking: métricas individuais por jogador e histórico de partidas por jogador
---
 
## 4. Stack tecnológica
 
| Camada | Tecnologia |
|---|---|
| App mobile | Android (Kotlin) |
| Backend | Django |
| Banco de dados | PostgreSQL |
| Autenticação | JWT + bcrypt - OAuth 2.0 Google - OAuth 2.0 Microsoft |
| Documentação da API | Swagger / OpenAPI |
| Controle de versão | Git + GitHub |
 
---
 
## 5. Estrutura do backlog
 
O backlog foi estruturado com épicos, features e histórias de usuário, priorizados de acordo com o sequenciador da Lean Inception:
 
- **MF-64 MVP: Jogador** — perfil do jogador, lado e nível de jogo
- **MF-18 MVP: Desafios e Recompensas** — criar, aceitar, cancelar, registrar resultado, resgatar recompensa
- **MF-19 Incremento 1: Ranking** — métricas individuais por jogador e histórico de partidas por jogador

A Definition of Ready (DoR) e a Definition of Done (DoD) foram definidas e aplicadas a todas as histórias da Sprint 1.
 
---
 
 
 
| Persona | Perfil | Principal necessidade |
|---|---|---|
| Gabriel | Aluno jogador, 36 anos | Desafiar adversários em dupla, ganhar recompensas reais e acompanhar sua evolução |
 
---
 
## 6. Estrutura do repositório
 
```
/
├── canvas-url.txt
├── LICENSE     
├── product-backlog.pdf      
├── sprint-backlog.pdf     
├── README.md  
├── wireframes/
│   ├── 01-criar-desafio.png
│   ├── 02-aceitar-recusar.png
│   ├── 03-detalhe-cancelar.png
│   ├── 04-registrar-resultado.png
│   ├── 05-resgatar-recompensa.png
│   └── 06-perfil-jogador.png
└── video-url.txt
```
 
---
 
*FuteVôlei Hub — MVP Acadêmico. PUC-Rio, Pós-Graduação em Engenharia de Software.*