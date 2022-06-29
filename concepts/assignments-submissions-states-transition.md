---
title: Estados, transições e limitações para atribuições e envios
description: Saiba mais sobre as alterações nos estados de atribuição e envio durante o fluxo do processo e quais APIs de educação no Microsoft Graph estão envolvidas.
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: conceptualPageType
ms.openlocfilehash: 479acbfa696c17d63e31c3298f10bedcfae906d9
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437055"
---
# <a name="states-transitions-and-limitations-for-assignments-and-submissions-in-microsoft-graph"></a>Estados, transições e limitações para atribuições e envios no Microsoft Graph

As tarefas e envios são uma parte importante na interação entre as ações de professores e alunos. Este artigo descreve as alterações nos estados de atribuição e envio durante o fluxo do processo e quais APIs de educação no Microsoft Graph estão envolvidas.

## <a name="assignment-states-and-transitions"></a>Estados de atribuição e transições

Uma tarefa representa uma tarefa ou unidade de trabalho atribuída a um aluno ou membros da equipe em uma classe como parte de seu estudo. Somente professores ou proprietários de equipe podem criar, copiar ou agendar tarefas. Essas ações têm um impacto nos estados de atribuição. A tabela a seguir lista os estados de atribuição e as APIs que estão disponíveis para alterar o estado. 

| Estado | Descrição | Chamada à API REST | Recursos disponíveis para edição |
|:--|:--|:--|:--|
| Rascunho | Status inicial quando uma nova atribuição é criada ou copiada de uma atribuição existente. | `POST /education/classes/{id}/assignments` | Recursos, categorias, rubricas |
| Published | Um estado de processamento em segundo plano quando a tarefa é distribuída para cada aluno atribuído. | `POST /education/classes/{id}/assignments/{id}/publish` | |
| Agendada | Status quando o professor agendou a tarefa para publicar em uma hora futura. | `PATCH /education/classes/{id}/assignments/{id}`<br/>`POST /education/classes/{id}/assignments/{id}/publish` | Recursos, categorias, rubricas |
| Atribuído | Depois de concluir a publicação, a tarefa é movida para o estado Atribuído e está disponível para os alunos. | `POST /education/classes/{id}/assignments/{id}/publish` | Envios |
| Pending | Status de processamento em segundo plano quando uma nova atribuição está sendo copiada de uma existente. | `POST /education/classes/{id}/assignments/{id}/copy`<br/>`PATCH /education/classes/{id}/assignments/{id}` | |

O diagrama a seguir mostra as transições de estado que podem ocorrer para atribuições.

![Diagrama de transições de estados de atribuição](images/states-transitions/diagram-assignments.PNG)

### <a name="how-to-verify-that-an-assignment-is-published"></a>Como verificar se uma atribuição foi publicada

O chamador deve usar a operação [de atribuição GET](/graph/api/educationassignment-get.md) para verificar o status atual da atribuição e verificar se o processo de publicação foi bem-sucedido.

### <a name="assignment-state-transitions-based-on-the-allowed-actions"></a>Transições de estado de atribuição com base nas ações permitidas

| Estado atual da atribuição | Nova ação | Novo estado |
|:--|:--|:--|
| Rascunho | O professor agenda a tarefa | Agendada |
| Rascunho | Publicar | Published |
| Rascunho | Edição | Rascunho |
| Rascunho | Descartado | |
| Published | Publicação concluída | Atribuído |
| Published | Falha na publicação | Rascunho |
| Published | Descartado | |
| Agendada | Data de conclusão do alcance | Published |
| Agendada | Cancelar agendamento | Rascunho |
| Agendada | Remarcar | Agendada |
| Atribuído | Descartado | |
| Pending | Cópia concluída | Rascunho |
| Pending | Descartado | |

> [!NOTE]
> Qualquer ação e transição de estado não listadas na tabela não é permitida.

### <a name="sync-vs-async-operations-over-assignments-api-calls"></a>Sincronizar versus operações assíncronas em chamadas à API de atribuições

A tabela a seguir menciona as chamadas à API que afetam o estado de atribuição e o tipo de operação.

As operações síncronas são executadas uma por vez e somente quando uma operação é concluída pode iniciar a operação a seguir e o resultado é retornado até que a última operação seja concluída. Com operações assíncronas, a operação é iniciada e outra operação pode ser executada antes da conclusão da anterior. A operação assíncrona executa alguma atividade em segundo plano e o chamador deve estar sondando para obter o resultado.

| API | Sincronizar ou assincronizar | Mecanismo para obter o estado mais recente |
|:--|:--|:--|
| `DELETE /education/classes/{id}/assignments/{id}` | Async | Enquete |
| `POST /education/classes/{id}/assignments/{id}/publish` | Async | Enquete |
| `PATCH /education/classes/{id}/assignments/{id}` | Async | Enquete |
| `POST /education/classes/{id}/assignments` | Async | Enquete |

## <a name="submission-states-and-transitions"></a>Estados de envio e transições

Um envio representa os recursos que um indivíduo (ou grupo) reveza para uma atribuição. Os envios pertencem a uma atribuição e são criados automaticamente quando uma atribuição é publicada.

O status é uma propriedade somente leitura no envio e é alterado com base nas ações de alunos e professores.

| Estado | Descrição | Chamada à API REST |
|:--|:--|:--|
| Trabalhando | Estado inicial após a criação do envio. | `POST /education/classes/{id}/assignments`<br/>`POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit` |
| Submitted | Isso acontece depois que o aluno entregou a tarefa. | `POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit` |
| Retornado | Depois que o professor devolveu a tarefa ao aluno. | `POST /education/classes/{id}/assignments/{id}/submissions/{id}/return` |
| Reatribuída | Depois que o professor retornou a tarefa ao aluno para revisão. | `POST /education/classes/{id}/assignments/{id}/submissions/{id}/reassign` |

O diagrama a seguir mostra o fluxo de transição de estado.

![Diagrama de transições de estados de envio](images/states-transitions/diagram-submissions.PNG)

### <a name="submission-state-transitions-based-on-allowed-actions"></a>Transições de estado de envio com base em ações permitidas

| Estado de envio atual | Nova ação | Novo estado |
|:--|:--|:--|
| Trabalhando | Entregar | Submitted |
| Trabalhando | Retornar para revisão | Reatribuída |
| Trabalhando | retornar | Retornado |
| Submitted | Desfazer Entregar | Trabalhando |
| Submitted | retornar | Retornado |
| Submitted | Retornar para revisão | Reatribuída |
| Retornado | Entregar | Submitted |
| Retornado | retornar | Retornado |
| Retornado | Retornar para revisão | Reatribuída |
| Reatribuída | Entregar | Submitted |
| Reatribuída | retornar | Retornado |
| Reatribuída | Retornar para revisão | Reatribuída |

> [!NOTE]
> Qualquer ação e transição de estado não listadas na tabela não é permitida.

### <a name="sync-vs-async-operations-over-submissions-api-calls"></a>Sincronizar versus operações assíncronas em chamadas à API de envios

A tabela a seguir lista as chamadas à API que afetam o estado de envio e o tipo de operação.

Nesse caso, todas as chamadas são assíncronas, o que significa que a operação é iniciada e outra operação pode ser iniciada antes que a primeira seja concluída. A operação assíncrona executa alguma atividade em segundo plano e o chamador deve estar sondando para obter o resultado.  

| API | Sincronizar ou assincronizar | Mecanismo para obter o estado mais recente |
|:--|:--|:--|
| `POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit` | Async | Enquete |
| `POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit` | Async | Enquete |
| `POST /education/classes/{id}/assignments/{id}/submissions/{id}/return` | Async | Enquete |
| `POST /education/classes/{id}/assignments/{id}/submissions/{id}/reassign` | Async | Enquete |

### <a name="limits"></a>Limites

Os seguintes limites se aplicam a todas as chamadas à API:

* O número máximo de recursos de tarefas e envios é 10 para o professor e mais 10 para o aluno.
* O tamanho máximo permitido para recursos é de 50 MB no geral ou 10 recursos.
* Os limites de limitação se aplicam; para obter detalhes, consulte [as diretrizes de limitação do Microsoft Graph](/graph/throttling).
