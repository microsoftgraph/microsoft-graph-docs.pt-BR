---
title: Estados, transições e limitações para atribuições e envios no Microsoft Graph
description: Este artigo descreve as alterações nos estados de atribuição e envio durante o fluxo de processo e quais APIs de educação na Microsoft Graph estão envolvidas.
localization_priority: Normal
author: cristobal-buenrostro
ms.prod: education
doc_type: conceptualPageType
ms.openlocfilehash: 98a283b02ddacdf05d4ffd20e8dd6cf436d256d3
ms.sourcegitcommit: f99dc2b6c8b4cb6f9f74cd780dccc47a2bccfaa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2021
ms.locfileid: "58668050"
---
# <a name="states-transitions-and-limitations-for-assignments-and-submissions-in-microsoft-graph"></a>Estados, transições e limitações para atribuições e envios no Microsoft Graph

Atribuições e envios são uma parte importante na interação entre as ações dos professores e dos alunos. Este artigo descreve as alterações nos estados de atribuição e envio durante o fluxo de processo e quais APIs de educação na Microsoft Graph estão envolvidas.

## <a name="assignment-states-and-transitions"></a>Estados de atribuição e transições

Uma atribuição representa uma tarefa ou unidade de trabalho atribuída a um aluno ou membros da equipe em uma classe como parte de seu estudo. Somente professores ou proprietários de equipe podem criar, copiar ou agendar atribuições. Essas ações têm impacto nos estados de atribuição. A tabela a seguir lista os estados de atribuição e as APIs disponíveis para alterar o estado. 

| Estado | Descrição | Chamada da API REST |
|:--|:--|:--|
| Rascunho | Status inicial quando uma nova atribuição é criada ou copiada de uma atribuição existente. | `POST /education/classes/{id}/assignments` |
| Published | Um estado de processamento em segundo plano quando a atribuição é distribuída a cada aluno atribuído. | `POST /education/classes/{id}/assignments/{id}/publish` |
| Agendada | Status quando o professor agendou a atribuição para publicar em uma hora futura. | `PATCH /education/classes/{id}/assignments/{id}`<br/>`POST /education/classes/{id}/assignments/{id}/publish` |
| Atribuído | Depois de concluir a publicação, a atribuição é movida para o estado Atribuído e está disponível para os alunos. | `POST /education/classes/{id}/assignments/{id}/publish` |
| Pending | Status do processamento em segundo plano quando uma nova atribuição está sendo copiada de uma tarefa existente. | `POST /education/classes/{id}/assignments/{id}/copy`<br/>`PATCH /education/classes/{id}/assignments/{id}` |

O diagrama a seguir mostra as transições de estado que podem ocorrer para atribuições.

![Diagrama de transições de estados de atribuição](images/states-transitions/diagram-assignments.PNG)

### <a name="how-to-verify-that-an-assignment-is-published"></a>Como verificar se uma atribuição foi publicada
O chamador deve usar a operação de atribuição GET t o verificar o status de atribuição atual e verificar se o processo de publicação foi bem-sucedido.

### <a name="assignments-states-transitions-based-on-the-allowed-actions"></a>Estados de atribuições transições com base nas ações permitidas
| Estado atual da atribuição | Ação | Novo estado |
|:--|:--|:--|
| Rascunho | O professor define uma data de vencimento. | Agendada |
| Rascunho | Publicar | Published |
| Rascunho | Editado | Rascunho |
| Rascunho | Descartado | | 
| Published | Publicar concluído | Atribuído |
| Published | Descartado | |
| Agendada | Alcançar a data de vencimento | Published |
| Agendada | Cancelar agendamento | Rascunho |
| Agendada | Reagendar | Agendada |
| Atribuído | Descartado | |
| Pending | Cópia concluída | Rascunho |
| Pending | Descartado | |   

`Note: Any action and state transition not listed in the table is NOT allowed`

### <a name="sync-vs-async-operations-over-assignments-api-calls"></a>Sincronizar versus operações assíncronas em chamadas de API de atribuições
A tabela a seguir menciona as chamadas de API que afetam o estado de atribuição e o tipo de operação.

Operações síncronas são executadas uma de cada vez e somente quando uma operação é concluída pode iniciar a operação a seguir e o resultado é retornado até que a última operação seja concluída. Com operações assíncronas, a operação é iniciada e outra operação pode ser executado antes da finalização da operação anterior. A operação assíncrona executa alguma atividade em segundo plano, e o chamador deve estar sondando para obter o resultado.

| API | Sincronizar ou assíncrono | Mecanismo para obter o estado mais recente |
|:--|:--|:--|
| `DELETE /education/classes/{id}/assignments/{id}` | Async | Sondagem |
| `POST /education/classes/{id}/assignments/{id}/publish` | Async | Sondagem |
| `PATCH /education/classes/{id}/assignments/{id}` | Async | Sondagem |
| `POST /education/classes/{id}/assignments` | Async | Sondagem |

## <a name="submission-states-and-transitions"></a>Estados de envio e transições

Um envio representa os recursos que um indivíduo (ou grupo) entrega para uma atribuição. Os envios pertencem a uma atribuição e são criados automaticamente quando uma atribuição é publicada.

O status é uma propriedade somente leitura no envio e muda com base nas ações de alunos e professores.
 

| Estado | Descrição | Chamada da API REST |
|:--|:--|:--|
| Trabalhando | Estado inicial após a criação do envio. | `POST /education/classes/{id}/assignments`<br/>`POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit` |
| Submitted | Isso acontece depois que o aluno se transforma na atribuição. | `POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit` |
| Retornado | Depois que o professor retornou a atribuição ao aluno. | `POST /education/classes/{id}/assignments/{id}/submissions/{id}/return` |

O diagrama a seguir mostra o fluxo de transição de estado.

![Diagrama de transições de estados de envio](images/states-transitions/diagram-submissions.PNG)

### <a name="submissions-states-transitions-based-on-allowed-actions"></a>Transições de estados de envios com base em ações permitidas
| Estado atual do envio | Ação | Novo estado |
|:--|:--|:--|
| Trabalhando | Ativar | Submitted |
| Trabalhando | retornar | Retornado |
| Submitted | Desfazer a ida e volta | Trabalhando |
| Submitted | retornar | Retornado |
| Retornado | Ativar | Submitted |

`Note: Any action and state transition not listed in the table is NOT allowed`

### <a name="sync-vs-async-operations-over-submissions-api-calls"></a>Sincronizar versus operações assíncronas em chamadas de API de envios
A tabela a seguir lista as chamadas de API que afetam o estado de envio e o tipo de operação.

Nesse caso, todas as chamadas são assíncronas, o que significa que a operação é iniciada e outra operação pode ser iniciada antes que a primeira termine. A operação assíncrona executa alguma atividade em segundo plano, e o chamador deve estar sondando para obter o resultado.  

| API | Sincronizar ou assíncrono | Mecanismo para obter o estado mais recente |
|:--|:--|:--|
| `POST /education/classes/{id}/assignments/{id}/submissions/{id}/submit` | Async | Sondagem |
| `POST /education/classes/{id}/assignments/{id}/submissions/{id}/unsubmit` | Async | Sondagem |
| `POST /education/classes/{id}/assignments/{id}/submissions/{id}/return` | Async | Sondagem |

### <a name="limits"></a>Limites
Os seguintes limites se aplicam a todas as chamadas de API:

* O número máximo de recursos de atribuições e envios é 10 para o professor e mais 10 para o aluno.
* O tamanho máximo permitido para recursos é de 50 MB ou 10 recursos.
* Limites de limitação se aplicam; para obter detalhes, consulte [Diretrizes](https://docs.microsoft.com/graph/throttling)de Graph de Graph da Microsoft.
