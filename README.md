# Análise de Levantamento de Requisitos — TodoMVC

## Introdução

Este repositório documenta o levantamento e a análise de requisitos realizado sobre a aplicação [TodoMVC (React)](https://todomvc.com/examples/react/#/), uma aplicação web de gerenciamento de tarefas usada como referência para estudo e prática de análise de software.

O objetivo do exercício é identificar e documentar os requisitos funcionais e não funcionais da aplicação a partir da observação direta do comportamento do sistema, simulando uma atividade real de levantamento de requisitos que antecede a criação de casos de teste.

## Sobre a Aplicação

A aplicação TodoMVC é uma lista de tarefas (to-do list) desenvolvida em React, acessível via navegador sem necessidade de login ou instalação. Ela permite criar, gerenciar e filtrar tarefas de forma simples e direta.

Acesse: [https://todomvc.com/examples/react/#/](https://todomvc.com/examples/react/#/)

## Funcionalidades Identificadas

### Tela Inicial

A tela inicial apresenta um campo de texto centralizado com o placeholder `What needs to be done?`, onde o usuário pode digitar uma nova tarefa. Enquanto não há tarefas cadastradas, o rodapé com filtros e contagem não é exibido.

<img src="https://github.com/IngridVanzeli/Analise_Requisitos/assets/47196643/ca3fd526-1157-4cac-add3-324b700861fd" width="500"/>

---

### Adicionar Itens

O usuário digita o texto da tarefa no campo principal e pressiona `Enter` para adicioná-la à lista. Cada tarefa adicionada aparece como um item na lista, acompanhada de um checkbox à esquerda para marcá-la como concluída.

<img src="https://github.com/IngridVanzeli/Analise_Requisitos/assets/47196643/7f9d1011-692b-48e3-859e-4f7af4a7864b" width="500"/>

---

### Filtros da Tela

O rodapé da aplicação exibe três filtros de visualização das tarefas:

- **All** — exibe todas as tarefas cadastradas, independente do status
- **Active** — exibe apenas as tarefas ainda não concluídas
- **Completed** — exibe apenas as tarefas marcadas como concluídas

O filtro ativo é destacado visualmente com uma borda ao redor do texto. O rodapé também exibe a contagem de itens ainda ativos (ex: `2 items left`).

<img src="https://github.com/IngridVanzeli/Analise_Requisitos/assets/47196643/5078504d-abf4-4641-9579-51275feb09ed" width="500"/>

---

### Concluir e Limpar Tarefas

O usuário pode marcar uma tarefa como concluída clicando no checkbox ao lado dela. Tarefas concluídas recebem uma formatação diferenciada (texto riscado). Quando há ao menos uma tarefa concluída, o botão **Clear completed** é exibido no rodapé, permitindo remover todas as tarefas concluídas de uma só vez.

Também é possível marcar todas as tarefas como concluídas simultaneamente clicando na seta `❯` exibida à esquerda do campo de entrada.

<img src="https://github.com/IngridVanzeli/Analise_Requisitos/assets/47196643/cee7ddbc-69e2-4bdf-9cce-97f9765586b6" width="500"/>

---

## Requisitos Levantados

### Requisitos Funcionais

| ID | Requisito |
|----|-----------|
| RF01 | O sistema deve permitir adicionar uma nova tarefa ao pressionar `Enter` após digitar no campo de texto |
| RF02 | O sistema deve exibir todas as tarefas cadastradas em ordem de criação |
| RF03 | O sistema deve permitir marcar uma tarefa como concluída por meio de um checkbox |
| RF04 | O sistema deve permitir desmarcar uma tarefa concluída, retornando-a ao status ativo |
| RF05 | O sistema deve exibir a contagem de tarefas ativas no rodapé (ex: `2 items left`) |
| RF06 | O sistema deve permitir filtrar as tarefas por status: **All**, **Active** e **Completed** |
| RF07 | O sistema deve destacar visualmente o filtro ativo |
| RF08 | O sistema deve exibir o botão **Clear completed** somente quando houver ao menos uma tarefa concluída |
| RF09 | O sistema deve remover todas as tarefas concluídas ao clicar em **Clear completed** |
| RF10 | O sistema deve permitir marcar todas as tarefas como concluídas simultaneamente por meio do botão de toggle geral |
| RF11 | O sistema deve aplicar formatação visual diferenciada (texto riscado) nas tarefas concluídas |
| RF12 | O sistema deve ocultar o rodapé (filtros e contagem) quando não houver nenhuma tarefa cadastrada |

### Requisitos Não Funcionais

| ID | Requisito |
|----|-----------|
| RNF01 | A aplicação deve funcionar diretamente no navegador, sem necessidade de instalação ou login |
| RNF02 | A interface deve ser responsiva e de uso intuitivo, sem necessidade de instruções para operação básica |
| RNF03 | As tarefas devem persistir durante a sessão do navegador, sem recarregar a página |

## Objetivo do Levantamento

Este exercício faz parte do estudo de análise de requisitos aplicada à qualidade de software. O levantamento de requisitos a partir da aplicação é uma etapa fundamental para:

- Entender o comportamento esperado do sistema antes de criar casos de teste
- Identificar regras de negócio implícitas que podem não estar documentadas
- Mapear cenários de sucesso e de erro que devem ser cobertos pelos testes
- Praticar a escrita de requisitos funcionais e não funcionais de forma clara e objetiva
<h4>Tela Inicial</h4>
<img src="https://github.com/IngridVanzeli/Analise_Requisitos/assets/47196643/ca3fd526-1157-4cac-add3-324b700861fd" width="400"/>

<h4>Adicionar Itens</h4>
<img src="https://github.com/IngridVanzeli/Analise_Requisitos/assets/47196643/7f9d1011-692b-48e3-859e-4f7af4a7864b" width="400"/>

<h4>Filtros da Tela</h4>
<img src="https://github.com/IngridVanzeli/Analise_Requisitos/assets/47196643/5078504d-abf4-4641-9579-51275feb09ed"width="400"/>

<h4>Concluir e Limpar Tarefas</h4>
<img src="https://github.com/IngridVanzeli/Analise_Requisitos/assets/47196643/cee7ddbc-69e2-4bdf-9cce-97f9765586b6" width="400"/>
