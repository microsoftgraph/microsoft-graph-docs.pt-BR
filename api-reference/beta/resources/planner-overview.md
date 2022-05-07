---
title: Usar a API REST do Planner
description: É possível usar a API do Planner no Microsoft Graph para criar e atribuir tarefas aos usuários em um grupo no Microsoft 365.
author: TarkanSevilmis
ms.localizationpriority: high
ms.prod: planner
doc_type: conceptualPageType
ms.openlocfilehash: db63a6a93a6290a368d7aa8eda3254f860ee780f
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247053"
---
# <a name="use-the-planner-rest-api"></a>Usar a API REST do Planner

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

É possível usar a API do Planner no Microsoft Graph para criar e atribuir tarefas aos usuários em um grupo no Microsoft 365.

Antes de começar a experimentar a API do Planner, vale a pena entender como os principais objetos na API do Planner se relacionam entre si e também com os grupos do Microsoft 365.

## <a name="plan-containers"></a>Planejar contêineres
No Planner, os planos estão sempre contidos em outro recurso. O recurso contido determina as regras de autorização do plano e todas as tarefas nele contidas, bem como o ciclo de vida do plano. Por exemplo, para planos contidos por grupos do Microsoft 365, os membros do grupo serão capazes de criar, editar, resolver e excluir tarefas no plano, bem como alterar algumas propriedades de nível de plano, como o nome do plano ou nomes de rótulos. Além disso, quando o grupo é excluído, todos os planos do grupo são excluídos automaticamente ou, se um grupo for restaurado, todos os planos serão restaurados automaticamente.

O tipo mais comum de contêiner é um grupo Microsoft 365.

### <a name="container-type-microsoft-365-groups"></a>Tipo de contêiner: grupos Microsoft 365

Os planos geralmente estão contidos em grupos do Microsoft 365 na API do Planner.
Para [obter os planos pertencentes a um grupo](../api/plannergroup-list-plans.md), faça a seguinte solicitação HTTP.

``` http
GET /groups/{group-id}/planner/plans
```

Ao [criar um novo plano](../api/planner-post-plans.md), torne um grupo seu contêiner definindo a propriedade `container` em um objeto de plano. Os planos devem ser contidos por um recurso suportado.

>**Observação:** o usuário que está criando o plano deve ser membro do grupo que conterá o plano. Ao criar um novo grupo usando [Criar grupo](../api/group-post-groups.md), você não é adicionado ao grupo como membro. Depois que o grupo for criado, adicione a si mesmo como membro usando [membros de postagem do grupo](../api/group-post-members.md).

## <a name="plans"></a>Planos

Os [planos](plannerplan.md) são os contêineres das [tarefas](plannertask.md).
Para [criar uma tarefa em um plano](../api/planner-post-tasks.md), defina a propriedade `planId` no objeto da tarefa como a ID do plano ao criar a tarefa.
No momento, as tarefas não podem ser criadas sem planos.
Para [recuperar as tarefas em um plano de](../api/plannerplan-list-tasks.md), faça a solicitação HTTP a seguir.

``` http
GET /planner/plans/{plan-id}/tasks
```

## <a name="tasks"></a>Tarefas

Cada tarefa pode ser atribuída a um usuário ao adicionar uma [atribuição](plannerassignment.md) à propriedade [assignments](plannerassignments.md) no objeto task. A ID do usuário ao qual a tarefa será atribuída é o nome da propriedade open em `assignments`. Além disso, a propriedade `orderHint` na atribuição deve ser especificada.

## <a name="task-and-plan-details"></a>Detalhes de planos e tarefas

Os recursos do Planner são organizados em objetos básicos e objetos detalhados. Os objetos básicos oferecem acesso às propriedades comuns dos recursos, adequadas para modos de exibição de lista. No entanto, os objetos detalhados fornecem acesso a grandes propriedades dos recursos, adequadas para modos de exibição de busca detalhada.

## <a name="visualization"></a>Visualização

Além do plano de dados e tarefas, a API do Planner também oferece recursos para criar uma visualização comum de dados nos clientes. Há vários tipos de visualização de dados disponíveis para as tarefas, conforme listado na tabela a seguir.

| As tarefas são exibidas como                                                                        | As tarefas são ordenadas com informações de                                         |
| :---------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------ |
| Lista plana (tarefas em um plano)                                                               | Propriedade `orderHint` em tarefas                                                   |
| Lista plana (tarefas atribuídas a um usuário)                                                      | Propriedade `assigneePriority` em tarefas                                            |
| Modo de exibição de quadro com colunas para os destinatários (atribuídos ao quadro de tarefas)                            | Objeto [assignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md) |
| O modo de exibição de quadro com colunas para o andamento da tarefa na direção de conclusão (quadro de tarefa de andamento) | Objeto [progressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)     |
| Modo de exibição de quadro com colunas personalizadas de tarefas (quadro de tarefa do bucket):                              | Objeto [bucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)         |

As colunas personalizadas no quadro de tarefas do bucket são representadas pelos objetos [bucket](plannerbucket.md) e, sua ordem, pela propriedade `orderHint` no objeto.

Toda a ordem é controlada pelos princípios descritos em [Dicas de ordem do Planner](planner-order-hint-format.md).

## <a name=""></a><a name="delta">Controlar alterações usando a consulta delta</a>

A consulta delta do Planner dá suporte a objetos consulta nos quais o usuário está inscrito.

Os usuários ficam inscritos nos seguintes objetos.

| Tipo de recurso do Planner | Instâncias assinadas                                                                                                                                                                                    |
| :-------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Tarefas                 | <ul><li>Criadas pelo usuário</li><li>Atribuídas ao usuário</li><li>Pertencentes a um plano que o usuário possui</li><li>Contidas em um plano compartilhado com o usuário por meio da coleção **SharedWith** do plano</li> |
| Planos                 | <ul><li>Compartilhado com o usuário por meio da coleção **SharedWith** do plano</li></ul>                                                                                                                     |
| Buckets               | <ul><li>Contidas em um plano compartilhado com o usuário por meio da coleção **SharedWith** do plano</li></ul>                                                                                                 |

### <a name=""></a><a name="objectcache">Preencher o cache de objetos para consultas delta</a>

Se quiser usar a API de consulta delta do Planner, mantenha um cache local de objetos nos quais o usuário está interessado em observar para aplicar as alterações do feed de resposta delta.

Os tipos de objetos de conteúdo delta que a consulta delta do Planner pode retornar atualmente serão:

* [plannerTask](plannertask.md)
* [plannerTaskDetails](plannertaskdetails.md)
* [plannerPlan](plannerplan.md)
* [plannerPlanDetails](plannerplandetails.md)
* [plannerBucket](plannerbucket.md)
* [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)
* [plannerBucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)
* [plannerAssignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md)

Use os métodos `GET` correspondente nos recursos para obter o estado inicial de objetos a ser preenchido no cache local.

### <a name="differentiating-between-object-creation-and-object-modification"></a>Diferenciar entre a criação de objeto e a modificação de objeto

Em determinados cenários, o autor da chamada pode querer distinguir entre a criação de objeto e a modificação do objeto dentro do feed de consulta delta do Planner.

Essas diretrizes podem ser usadas para inferir a criação do objeto:

* A propriedade `createdBy` só aparecerá em objetos recém-criados.
* Um objeto `plannerTask` recém-criado será seguido pelo seu objeto `plannerTaskDetails` correspondente.
* Um objeto `plannerPlan` recém-criado será seguido pelo seu objeto `plannerPlanDetails` correspondente.

### <a name="usage"></a>Uso

O autor da chamada deve ter um cache que contenha objetos inscritos. Para obter detalhes sobre como preencher o cache local de objetos inscritos, confira [Preencher o cache de objetos para consultas delta](#populate-the-object-cache-for-delta-queries).

O fluxo de chamadas da consulta delta do Planner é assim:

1. O autor da chamada inicia uma consulta de sincronização delta, obtendo um `@odata.nextLink` e uma coleção de alterações vazia.
2. O autor da chamada deve [preencher o cache do objeto para consultas delta](#populate-the-object-cache-for-delta-queries) com objetos nos quais o usuário esteja inscrito, atualizando o cache.
3. O autor da chamada segue o `@odata.nextLink` fornecido na consulta de sincronização delta inicial para obter um novo `@odata.deltaLink` para alterações desde a etapa anterior.
4. O autor da chamada aplica as alterações da resposta delta retornada nos objetos em seu cache.
5. O autor da chamada segue o novo deltaLink para obter o próximo deltaLink e alterações desde que o `@odata.deltaLink` atual foi gerado.
6. O autor da chamada aplica as alterações (caso existam) e espera um pouco antes de executar novamente as etapas anterior e atual.

## <a name="planner-resource-versioning"></a>Versão do recurso do Planner

O Planner cria versões de todos os recursos usando **etags**. Esses **etags** são retornados com a propriedade `@odata.etag` em cada recurso. As solicitações `PATCH` e `DELETE` requerem que a última **etag** conhecida pelo cliente seja especificada com um cabeçalho `If-Match`.
O Planner permite alterações em versões mais antigas de recursos, se a alteração pretendida não estiver em conflito com as alterações mais recentes aceitas pelo serviço do Planner no mesmo recurso. Os clientes podem identificar qual **etag** para o mesmo recurso é mais recente ao calcular qual valor de **etag** é maior em comparação com a cadeia de caracteres ordinal.
Cada recurso tem uma **etag** única. Não há comparações entre os valores de etags de recursos diferentes, incluindo aqueles com relações de confinamento.
Espera-se que os aplicativos cliente tratem dos controles de versão relacionados aos [códigos de erro](/graph/errors) **409** e **412** lendo a versão mais recente do item e resolvendo as alterações conflitantes.

## <a name="common-planner-error-conditions"></a>Condições de erro comuns do Planner

Além dos [erros gerais](/graph/errors) que se aplicam ao Microsoft Graph, algumas condições de erro são específicas da API do Planner.

### <a name="400-bad-request"></a>400 Solicitação Incorreta

Em alguns cenários comuns, as solicitações `POST` e `PATCH` podem retornar um código de status 400. Estas são algumas das mais comuns:

* As propriedades Open Type não têm os tipos corretos ou o tipo não foi especificado ou não contêm propriedades. Por exemplo, as propriedades plannerAssignments com valores complexos precisam declarar a propriedade  com valor .
* Os valores da dica de ordem não têm o formato correto. Por exemplo, um valor de dica de ordem está sendo definido diretamente como o valor retornado ao cliente.
* Os dados são ilogicamente inconsistentes. Por exemplo, a data de início da tarefa é posterior à data de conclusão da tarefa.

### <a name="403-forbidden"></a>403 Proibido

Além dos erros gerais, a API do Planner também retorna esse código de status 403 quando um limite definido pelo serviço é excedido. Se esse for o caso, a propriedade `code` no tipo de recurso do erro indicará o tipo do limite excedido pela solicitação.
Os valores possíveis para os tipos de limite são:

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
| MaximumFavoritePlansForUser   | A propriedade `favoritePlanReferences` no recurso [plannerUser](planneruser.md) contém muitos valores.                                                                                            |
| MaximumRecentPlansForUser     | A propriedade `recentPlanReferences` no recurso [plannerUser](planneruser.md) contém muitos valores.                                                                                              |
| MaximumContextsOnPlan         | A propriedade `contexts` no recurso [plannerPlan](plannerplan.md) contém muitos valores.                                                                                                          |
| MaximumPlannerPlans       | O grupo já contém um plano. Atualmente, os grupos só podem conter um plano. **Observação:** alguns aplicativos da Microsoft podem ultrapassar esse limite. Futuramente, essa funcionalidade será estendida para todos os aplicativos.                                                                                                      |

### <a name="412-precondition-failed"></a>412 Falha na Pré-condição

Todas as solicitações `POST`, `PATCH` e `DELETE` da API do Planner exigem que o cabeçalho `If-Match` seja especificado com o último valor de etag conhecido do recurso que está sujeito à solicitação.
O código de status 412 também pode ser retornado se o valor da etag especificado na solicitação já não corresponder a uma versão do recurso no serviço. Nesse caso, os clientes devem ler o recurso novamente e obter uma nova etag.

## <a name="whats-new"></a>O que há de novo
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

