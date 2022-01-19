---
title: Estados, transições e limitações para atribuições e envios no Microsoft Graph
description: Este artigo descreve as alterações nos estados de atribuição e envio durante o fluxo de processo e quais APIs de educação na Microsoft Graph estão envolvidas.
ms.localizationpriority: medium
author: cristobal-buenrostro
ms.prod: education
doc_type: conceptualPageType
ms.openlocfilehash: 456c2c8351521146f7160d65b6b0d2dff37d31dc
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072065"
---
# <a name="states-transitions-and-limitations-for-assignments-and-submissions-in-microsoft-graph"></a>Estados, transições e limitações para atribuições e envios no Microsoft Graph

Atribuições e envios são uma parte importante na interação entre as ações dos professores e dos alunos. Este artigo descreve as alterações nos estados de atribuição e envio durante o fluxo de processo e quais APIs de educação na Microsoft Graph estão envolvidas.

## <a name="assignment-states-and-transitions"></a>Estados de atribuição e transições

Uma atribuição representa uma tarefa ou unidade de trabalho atribuída a um aluno ou membros da equipe em uma classe como parte de seu estudo. Somente professores ou proprietários de equipe podem criar, copiar ou agendar atribuições. Essas ações têm impacto nos estados de atribuição. A tabela a seguir lista os estados de atribuição e as APIs disponíveis para alterar o estado. 

| Estado | Descrição | Chamada da API REST |
|:--|:--|:--|
| Rascunho | Status inicial quando uma nova atribuição é criada ou copiada de uma atribuição existente. | `POST /education/classes/{id}/assignments` |
| Publicado | Um estado de processamento em segundo plano quando a atribuição é distribuída a cada aluno atribuído. | `POST /education/classes/{id}/assignments/{id}/publish` |
| Agendada | Status quando o professor agendou a atribuição para publicar em uma hora futura. | `PATCH /education/classes/{id}/assignments/{id}`<br/>`POST /education/classes/{id}/assignments/{id}/publish` |
| Atribuído | Depois de concluir a publicação, a atribuição é movida para o estado Atribuído e está disponível para os alunos. | `POST /education/classes/{id}/assignments/{id}/publish` |
| Pendente | Status do processamento em segundo plano quando uma nova atribuição está sendo copiada de uma tarefa existente. | `POST /education/classes/{id}/assignments/{id}/copy`<br/>`PATCH /education/classes/{id}/assignments/{id}` |

O diagrama a seguir mostra as transições de estado que podem ocorrer para atribuições.

![Diagrama de transições de estados de atribuição](images/states-transitions/diagram-assignments.PNG)

### <a name="how-to-verify-that-an-assignment-is-published"></a>Como verificar se uma atribuição foi publicada
O chamador deve usar a operação [de atribuição GET](/graph/api/educationassignment-get.md) para verificar o status atual da atribuição e verificar se o processo de publicação foi bem-sucedido.

### <a name="assignments-states-transitions-based-on-the-allowed-actions"></a>Estados de atribuições transições com base nas ações permitidas
| Estado atual da atribuição | Ação | Novo estado |
|:--|:--|:--|
| Rascunho | O professor agenda a atribuição | Agendada |
| Rascunho | Publicar | Publicado |
| Rascunho | Editado | Rascunho |
| Rascunho | Descartado | | 
| Publicado | Publicar concluído | Atribuído |
| Publicado | Descartado | |
| Agendada | Alcançar a data de vencimento | Publicado |
| Agendada | Cancelar agendamento | Rascunho |
| Agendada | Reagendar | Agendada |
| Atribuído | Descartado | |
| Pendente | Cópia concluída | Rascunho |
| Pendente | Descartado | |   

`Note: Any action and state transition not listed in the table is NOT allowed`

### <a name="sync-vs-async-operations-over-assignments-api-calls"></a>Sincronizar versus operações assíncronas em chamadas de API de atribuições
A tabela a seguir menciona as chamadas de API que afetam o estado de atribuição e o tipo de operação.

Operações síncronas são executadas uma de cada vez e somente quando uma operação é concluída pode iniciar a operação a seguir e o resultado é retornado até que a última operação seja concluída. Com operações assíncronas, a operação é iniciada e outra operação pode ser executado antes da finalização da operação anterior. A operação assíncrona executa alguma atividade em segundo plano, e o chamador deve estar sondando para obter o resultado.

| API | Sincronizar ou assíncrono | Mecanismo para obter o estado mais recente |
|:--|:--|:--|
| `DELETE /education/classes/{id}/assignments/{id}` | Async | Enquete |
| `POST /education/classes/{id}/assignments/{id}/publish` | Async | Enquete |
| `PATCH /education/classes/{id}/assignments/{id}` | Async | Enquete |
| `POST /education/classes/{id}/assignments` | Async | Enquete |

## <a name="submission-states-and-transitions"></a>Estados de envio e transições

Um envio representa os recursos que um indivíduo (ou grupo) entrega para uma atribuição. Os envios pertencem a uma atribuição e são criados automaticamente quando uma atribuição é publicada.

O status é uma propriedade somente leitura no envio e muda com base nas ações de alunos e professores.
 

| Estado | Descrição | Chamada da API REST |
|:--|:--|:--|
| Trabalhando | Estado inicial após a criação do envio. | `POST /education/classes/{id}/assignments`<br/>`POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit` |
| Submitted | Isso acontece depois que o aluno foi transformado na atribuição. | `POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit` |
| Retornado | Depois que o professor retornou a atribuição ao aluno. | `POST /education/classes/{id}/assignments/{id}/submissions/{id}/return` |
| Reatribuido | Depois que o professor retornou a atribuição ao aluno para revisão. | `POST /education/classes/{id}/assignments/{id}/submissions/{id}/reassign` |

O diagrama a seguir mostra o fluxo de transição de estado.

![Diagrama de transições de estados de envio](images/states-transitions/diagram-submissions.PNG)

### <a name="submissions-states-transitions-based-on-allowed-actions"></a>Transições de estados de envios com base em ações permitidas
| Estado atual do envio | Ação | Novo estado |
|:--|:--|:--|
| Trabalhando | Ativar | Submitted |
| Trabalhando | Retornar para revisão | Reatribuido |
| Trabalhando | retornar | Retornado |
| Submitted | Desfazer a ida e volta | Trabalhando |
| Submitted | retornar | Retornado |
| Submitted | Retornar para revisão | Reatribuido |
| Retornado | Ativar | Submitted |
| Retornado | retornar | Retornado |
| Retornado | Retornar para revisão | Reatribuido |
| Reatribuido | Ativar | Submitted |
| Reatribuido | retornar | Retornado |
| Reatribuido | Retornar para revisão | Reatribuido |

`Note: Any action and state transition not listed in the table is NOT allowed`

### <a name="sync-vs-async-operations-over-submissions-api-calls"></a>Sincronizar versus operações assíncronas em chamadas de API de envios
A tabela a seguir lista as chamadas de API que afetam o estado de envio e o tipo de operação.

Nesse caso, todas as chamadas são assíncronas, o que significa que a operação é iniciada e outra operação pode ser iniciada antes que a primeira termine. A operação assíncrona executa alguma atividade em segundo plano, e o chamador deve estar sondando para obter o resultado.  

| API | Sincronizar ou assíncrono | Mecanismo para obter o estado mais recente |
|:--|:--|:--|
| `POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit` | Async | Enquete |
| `POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit` | Async | Enquete |
| `POST /education/classes/{id}/assignments/{id}/submissions/{id}/return` | Async | Enquete |
| `POST /education/classes/{id}/assignments/{id}/submissions/{id}/reassign` | Async | Enquete |

### <a name="limits"></a>Limites
Os seguintes limites se aplicam a todas as chamadas de API:

* O número máximo de recursos de atribuições e envios é 10 para o professor e mais 10 para o aluno.
* O tamanho máximo permitido para recursos é de 50 MB ou 10 recursos.
* Limites de limitação se aplicam; para obter detalhes, consulte [Diretrizes](/graph/throttling)de Graph de Graph da Microsoft.