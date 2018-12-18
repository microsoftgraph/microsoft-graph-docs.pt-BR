---
title: Use o Planejador de API REST
description: Você pode usar a API do planejador no Microsoft Graph criar tarefas e atribuí-las aos usuários em um grupo no Office 365.
author: TarkanSevilmis
ms.openlocfilehash: a72ec36eb116475a0cbc75a2161696d819e53985
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312065"
---
# <a name="use-the-planner-rest-api"></a>Use o Planejador de API REST

Você pode usar a API do planejador no Microsoft Graph criar tarefas e atribuí-las aos usuários em um grupo no Office 365.

Antes de começar com a API do planejador, convém entender como os objetos principais se relacionam entre si, bem como para grupos do Office 365.

## <a name="office-365-groups"></a>Grupos do Office 365

Grupos de Office 365 são os proprietários dos planos de na API do planejador.
Para [obter os planos pertencentes a um grupo](../api/plannergroup-list-plans.md), verifique a seguinte solicitação HTTP.

``` http
GET /groups/{id}/planner/plans
```

Quando [criar um novo plano](../api/planner-post-plans.md), tornar seu proprietário de um grupo, definindo o `owner` propriedade em um objeto do plano. Planos devem pertencer por grupos.

>**Observação:** O usuário que está criando o plano deve ser um membro do grupo que será o proprietário do plano. Quando você cria um novo grupo usando [Criar grupo](../api/group-post-groups.md), você não é adicionados ao grupo como um membro. Depois que o grupo é criado, adicione si mesmo como membro usando o [grupo postar membros](../api/group-post-members.md).

## <a name="plans"></a>Planos

[Planos](plannerplan.md) são os recipientes de [tarefas](plannertask.md). Para [criar uma tarefa em um plano](../api/planner-post-tasks.md), defina o `planId` propriedade no objeto de tarefa para a ID do plano durante a criação da tarefa.
Tarefas atualmente não podem ser criadas sem planos.
Para [recuperar as tarefas em um plano](../api/plannerplan-list-tasks.md), verifique a seguinte solicitação HTTP.

``` http
GET /planner/plans/{id}/tasks
```

## <a name="tasks"></a>Tarefas

Cada tarefa pode ser atribuída a um usuário ao adicionar uma [atribuição](plannerassignment.md) à propriedade [assignments](plannerassignments.md) no objeto task. A ID do usuário ao qual a tarefa será atribuída é o nome da propriedade open em `assignments`. Além disso, a propriedade `orderHint` na atribuição deve ser especificada.

## <a name="task-and-plan-details"></a>Detalhes de planos e tarefas 

Os recursos do Planner são organizados em objetos básicos e objetos detalhados. Os objetos básicos oferecem acesso às propriedades comuns dos recursos, adequadas para modos de exibição de lista. No entanto, os objetos detalhados fornecem acesso a grandes propriedades dos recursos, adequadas para modos de exibição de busca detalhada.

## <a name="visualization"></a>Visualização

Além dos dados de tarefa e plano, a API do planejador também fornece recursos para a criação de uma visualização comuns de dados entre clientes. Vários tipos de visualização de dados estão disponíveis para tarefas, conforme listado na tabela a seguir.

| As tarefas são exibidas como                                                                        | As tarefas são ordenadas com informações de                                         |
| :---------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------ |
| Lista plana (tarefas em um plano)                                                               | Propriedade `orderHint` em tarefas                                                   |
| Lista plana (tarefas atribuídas a um usuário)                                                      | Propriedade `assigneePriority` em tarefas                                            |
| Modo de exibição de quadro com colunas para os destinatários (atribuídos ao quadro de tarefas)                            | Objeto [assignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md) |
| O modo de exibição de quadro com colunas para o andamento da tarefa na direção de conclusão (quadro de tarefa de andamento) | Objeto [progressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)     |
| Modo de exibição de quadro com colunas personalizadas de tarefas (quadro de tarefa do bucket):                              | Objeto [bucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)         |

As colunas personalizadas no quadro de tarefas do bucket são representadas pelos objetos [bucket](plannerbucket.md) e, sua ordem, pela propriedade `orderHint` no objeto.

Todos os a ordenação é controlada pelos princípios descritos em [dicas de ordem Planejador](planner-order-hint-format.md).

## <a name="planner-resource-versioning"></a>Versão do recurso do Planner

Versões do planejador todos os recursos usando **etags**. Esses **etags** são retornadas com `@odata.etag` propriedade em cada recurso. `PATCH`e `DELETE` solicitações exige a última **etag** conhecidos pelo cliente seja especificado com um `If-Match` cabeçalho.
Planejador permite alterações versões mais antigas dos recursos, se a alteração pretendida não está em conflito com as alterações mais recentes aceitas pelo serviço Planejador no mesmo recurso. Os clientes podem identificar quais **etag** para o mesmo recurso é mais recente Calculando qual valor **etag** for maior em comparação ordinal da cadeia de caracteres. Cada recurso tem um exclusivo **etag**. Valores de ETag para recursos diferentes, incluindo aqueles com relações de confiança contenção, não podem ser comparados.
Os aplicativos cliente esperados para lidar com controle de versão de [códigos de erro](/graph/errors) **409** e **412** relacionados ao lendo a versão mais recente do item e resolver as alterações conflitantes.

## <a name="common-planner-error-conditions"></a>Condições de erro comuns do Planner

Além dos [erros gerais](/graph/errors) que se aplicam ao Microsoft Graph, algumas condições de erro são específicas da API do Planner.

### <a name="400-bad-request"></a>400 Solicitação Incorreta

Em alguns cenários comuns, `POST` e `PATCH` solicitações podem retornar um código de 400 status. A seguir estão algumas das causas comuns:

* As propriedades Open Type não têm os tipos corretos ou o tipo não foi especificado ou não contêm propriedades. Por exemplo, as propriedades [plannerAssignments](plannerassignments.md) com valores complexos precisam declarar a propriedade `@odata.type` com valor `microsoft.graph.plannerAssignment`.
* Os valores da dica de ordem não têm o [formato correto](planner-order-hint-format.md). Por exemplo, um valor de dica de ordem está sendo definido diretamente como o valor retornado ao cliente.
* Os dados são logicamente inconsistentes. Por exemplo, a data de início da tarefa é posterior à data de conclusão da tarefa.

### <a name="403-forbidden"></a>403 Proibido

Além dos erros gerais, a API do planejador também retorna o código de 403 status quando um limite definido pelo serviço foi excedido. Se este for o caso, o `code` propriedade no tipo de recurso de erro indicará o tipo do limite ultrapassado na solicitação.
A seguir estão os valores possíveis para os tipos de limite.

| Valor                         | Descrição                                                                                                                                                                                              |
| :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| MaximumProjectsOwnedByUser    | Foi excedido o número máximo de Planos pertencentes ao limite do grupo. Esse limite se baseia na propriedade `owner` no recurso [plannerPlan](plannerplan.md).                                         |
| MaximumProjectsSharedWithUser | Foi excedido o número máximo de Planos compartilhados com um limite de usuário.  Esse limite se baseia na propriedade `sharedWith` no recurso [plannerPlanDetails](plannerplandetails.md).                   |
| MaximumTasksCreatedByUser     | Foi excedido o número máximo de Tarefas criadas pelo limite do usuário. Esse limite se baseia na propriedade `createdBy` no recurso [plannerTask](plannertask.md).                                    |
| MaximumTasksAssignedToUser    | Foi excedido o número máximo de Tarefas atribuídas ao limite do usuário. Esse limite se baseia na propriedade `assignments` no recurso [plannerTask](plannertask.md).                                 |
| MaximumTasksInProject         | Foi excedido o número máximo de Tarefas no limite de um Plano. Esse limite se baseia na propriedade `planId` no recurso [plannerTask](plannertask.md).                                               |
| MaximumActiveTasksInProject   | Foi excedido o número máximo de Tarefas que não foram concluídas no limite de um Plano. Esse limite se baseia nas propriedades `planId` e `percentComplete` no recurso [plannerTask](plannertask.md). |
| MaximumBucketsInProject       | Foi excedido o número máximo de Buckets no limite de um Plano. Esse limite se baseia na propriedade `planId` no recurso [plannerBucket](plannerbucket.md).                                         |
| MaximumUsersSharedWithProject | A propriedade `sharedWith` no recurso [plannerPlanDetails](plannerplandetails.md) contém muitos valores.                                                                                          |
| MaximumReferencesOnTask       | A propriedade `references` no recurso [plannerTaskDetails](plannertaskdetails.md) contém muitos valores.                                                                                          |
| MaximumChecklistItemsOnTask   | A propriedade `checklist` no recurso [plannerTaskDetails](plannertaskdetails.md) contém muitos valores.                                                                                           |
| MaximumAssigneesInTasks       | A propriedade `assignments` no recurso [plannerTask](plannertask.md) contém muitos valores.                                                                                                       |
| MaximumPlannerPlans       | O grupo já contém um plano. Atualmente, os grupos podem conter somente um plano. **Observação:** Alguns aplicativos Microsoft podem exceder esse limite. No futuro, podemos estenderá esse recurso para todos os aplicativos.                                                                                                      |

### <a name="412-precondition-failed"></a>412 Falha na Pré-condição 

API de todos os Planer `POST`, `PATCH`, e `DELETE` solicitações exigem o `If-Match` cabeçalho seja especificado com o último valor conhecido etag do recurso que está sujeito a solicitação.
O código de 412 status também pode ser retornado se o valor de etag especificado na solicitação não corresponde a uma versão do recurso no serviço. Nesse caso, os clientes devem ler o recurso novamente e obter um novo etag.

