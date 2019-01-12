---
title: Use o Planejador de API REST
description: Você pode usar a API do planejador no Microsoft Graph criar tarefas e atribuí-las aos usuários em um grupo no Office 365.
author: TarkanSevilmis
localization_priority: Priority
ms.prod: planner
ms.openlocfilehash: 2995cfe32e921889a55ec56c67989ecdfc9716ed
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27942567"
---
# <a name="use-the-planner-rest-api"></a>Use o Planejador de API REST

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Você pode usar a API do planejador no Microsoft Graph criar tarefas e atribuí-las aos usuários em um grupo no Office 365.

Antes de começar com a API do planejador, será útil compreender como os objetos principais se relacionam entre si, bem como para grupos do Office 365.

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

## <a name="delta">Controlar alterações usando consulta delta</a>

Consulta de delta do planejador suporta consultando objetos que o usuário está inscrito.

Os usuários estão inscritos para os objetos a seguir.

| Tipo de recurso de Planejador | Instâncias inscritas                                                                                                                                                                                    |
| :-------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Tarefas                 | <ul><li>Criadas pelo usuário</li><li>Atribuída ao usuário</li><li>Pertencem a um plano de que o usuário possui</li><li>Contidos em um plano no compartilhados com o usuário por meio da coleção de **SharedWith** do plano</li> |
| Planos                 | <ul><li>Compartilhados com o usuário por meio da coleção de **SharedWith** do plano</li></ul>                                                                                                                     |
| Partições de memória               | <ul><li>Contidos em um plano no compartilhados com o usuário por meio da coleção de **SharedWith** do plano</li></ul>                                                                                                 |  |

### <a name="objectcache">Preencher o cache de objetos para consultas delta</a>

Se você quiser usar a API de consulta delta planejador, manter um cache local de objetos que o usuário está interessado em observando para aplicar as alterações a partir do feed de resposta delta.

Os objetos de carga de delta que a consulta de delta Planejador atualmente pode retornar será dos seguintes tipos:

* [plannerTask](plannertask.md)
* [plannerTaskDetails](plannertaskdetails.md)
* [plannerPlan](plannerplan.md)
* [plannerPlanDetails](plannerplandetails.md)
* [plannerBucket](plannerbucket.md)
* [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)
* [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)
* [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)

Use o correspondente `GET` métodos no recurso para obter o estado inicial dos objetos a serem preenchidos no cache local.

### <a name="differentiating-between-object-creation-and-object-modification"></a>Distinguir entre a criação do objeto e modificação de objeto

Em determinados cenários, o chamador talvez queira distinguir entre a criação do objeto e a modificação do objeto dentro da consulta de delta do planejador feed.

Estas diretrizes podem ser usadas para interpretar a criação do objeto:

* O `createdBy` propriedade aparecerá somente em objetos recentemente criados.
* Uma recém-criadas `plannerTask` objeto será seguido por correspondente `plannerTaskDetails` objeto.
* Uma recém-criadas `plannerPlan` objeto será seguido por correspondente `plannerPlanDetails` objeto.

### <a name="usage"></a>Uso

O chamador deve ter um cache que contém objetos inscritos. Para obter detalhes sobre como preencher o cache local de objetos inscritos, consulte [preencher o cache de objetos para consultas delta](#populate-the-object-cache-for-delta-queries).

Fluxo de chamadas de consulta do planejador delta é da seguinte maneira:

1. O chamador inicia uma consulta de sincronização delta, obtendo uma `nextLink` e uma coleção vazia das alterações.
2. O chamador deve [preencher o cache de objetos para consultas delta](#populate-the-object-cache-for-delta-queries) com objetos que o usuário está inscrito em, atualizando seu cache.
3. O chamador segue o `nextLink` fornecido na consulta sincronização delta inicial para obter uma nova `deltaLink` para quaisquer alterações desde a etapa anterior.
4. O chamador aplica as alterações na resposta delta retornado para os objetos em seu cache.
5. O chamador segue o novo deltaLink para obter o próximo deltaLink e altera desde atual `deltaLink` foi gerado.
6. O chamador aplica as alterações (se houver) e aguarda pouco antes de executar novamente o anterior etapa e esta etapa.

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
| MaximumFavoritePlansForUser   | O `favoritePlanReferences` propriedade no recurso [plannerUser](planneruser.md) contém muitos valores.                                                                                            |
| MaximumRecentPlansForUser     | O `recentPlanReferences` propriedade no recurso [plannerUser](planneruser.md) contém muitos valores.                                                                                              |
| MaximumContextsOnPlan         | O `contexts` propriedade no recurso [plannerPlan](plannerplan.md) contém muitos valores.                                                                                                          |
| MaximumPlannerPlans       | O grupo já contém um plano. Atualmente, os grupos podem conter somente um plano. **Observação:** Alguns aplicativos Microsoft podem exceder esse limite. No futuro, podemos estenderá esse recurso para todos os aplicativos.                                                                                                      |

### <a name="412-precondition-failed"></a>412 Falha na Pré-condição 

API de todos os Planer `POST`, `PATCH`, e `DELETE` solicitações exigem o `If-Match` cabeçalho seja especificado com o último valor conhecido etag do recurso que está sujeito a solicitação.
O código de 412 status também pode ser retornado se o valor de etag especificado na solicitação não corresponde a uma versão do recurso no serviço. Nesse caso, os clientes devem ler o recurso novamente e obter um novo etag.

