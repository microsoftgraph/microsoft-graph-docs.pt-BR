---
title: Usar a API REST do Planner
description: É possível usar a API do Planner no Microsoft Graph para criar e atribuir tarefas aos usuários em um grupo no Microsoft 365.
author: TarkanSevilmis
ms.localizationpriority: high
ms.prod: planner
doc_type: conceptualPageType
ms.openlocfilehash: cf17b796f8689467b04d1ea814192d1f499b15cc
ms.sourcegitcommit: ca1b33aaecb320b33423aeec7438ce306bffab14
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/14/2022
ms.locfileid: "65420702"
---
# <a name="use-the-planner-rest-api"></a>Usar a API REST do Planner

É possível usar a API do Planner no Microsoft Graph para criar e atribuir tarefas aos usuários em um grupo no Microsoft 365.

Antes de começar a experimentar a API do Planner, vale a pena entender como os principais objetos na API do Planner se relacionam entre si e também com os grupos do Microsoft 365.

## <a name="plan-containers"></a>Planejar contêineres
No Microsoft Planner, os planos estão sempre contidos por outro recurso. O recurso contido determina as regras de autorização do plano e de todas as tarefas nele contidas, bem como o ciclo de vida do plano. Por exemplo, para planos contidos por grupos do Microsoft 365, os membros do grupo serão capazes de criar, editar, resolver e excluir tarefas no plano, bem como alterar algumas propriedades de nível de plano, como o nome do plano ou nomes de rótulos. Além disso, quando o grupo é excluído, todos os planos do grupo são excluídos automaticamente ou, se um grupo for restaurado, todos os planos serão restaurados automaticamente.

O tipo mais comum de contêiner é um grupo Microsoft 365.

### <a name="container-type-microsoft-365-groups"></a>Tipo de contêiner: grupos Microsoft 365

Os planos geralmente estão contidos em grupos do Microsoft 365 na API do Planner.
Para [obter os planos pertencentes a um grupo](../api/plannergroup-list-plans.md), faça a seguinte solicitação HTTP.

``` http
GET /groups/{group-id}/planner/plans
```

Ao [criar um novo plano](../api/planner-post-plans.md), defina a propriedade do **contêiner** em um objeto de plano para fazer de um grupo seu contêiner. Os planos devem estar contidos em um recurso com suporte.

>**Observação:** o usuário que está criando o plano deve ser membro do grupo que conterá o plano. Ao criar um novo grupo usando [Criar grupo](../api/group-post-groups.md), você não é adicionado ao grupo como membro. Depois que o grupo for criado, adicione a si mesmo como membro usando [membros de postagem do grupo](../api/group-post-members.md).

## <a name="plans"></a>Planos

Os [planos](plannerplan.md) são os contêineres das [tarefas](plannertask.md).
Para [criar uma tarefa em um plano](../api/planner-post-tasks.md), defina a propriedade **planId** no objeto da tarefa como a ID do plano ao criar a tarefa.
No momento, as tarefas não podem ser criadas sem planos.
Para [recuperar as tarefas em um plano de](../api/plannerplan-list-tasks.md), faça a solicitação HTTP a seguir.

``` http
GET /planner/plans/{plan-id}/tasks
```

## <a name="tasks"></a>Tarefas

Cada tarefa pode ser atribuída a um usuário ao adicionar uma [tarefa](plannerassignment.md) na propriedade das [atribuições](plannerassignments.md) no objeto da tarefa. A ID do usuário ao qual a tarefa será atribuída é o nome da propriedade aberta em **tarefas**, e a propriedade **orderHint** na atribuição deve ser especificada.

## <a name="task-and-plan-details"></a>Detalhes de planos e tarefas 

Os recursos do Planner são organizados em objetos básicos e objetos detalhados. Os objetos básicos oferecem acesso às propriedades comuns dos recursos, adequadas para modos de exibição de lista. No entanto, os objetos detalhados fornecem acesso a grandes propriedades dos recursos, adequadas para modos de exibição de busca detalhada.

## <a name="visualization"></a>Visualização

Além do plano de dados e tarefas, a API do Planner também oferece recursos para criar uma visualização comum de dados nos clientes. Há vários tipos de visualização de dados disponíveis para as tarefas, conforme listado na tabela a seguir.

| As tarefas são exibidas como                                                                        | As tarefas são ordenadas com informações de                                         |
| :---------------------------------------------------------------------------------------- | :------------------------------------------------------------------------------ |
| Lista plana (tarefas em um plano)                                                               | Propriedade **orderHint** em tarefas                                                   |
| Lista plana (tarefas atribuídas a um usuário)                                                      | Propriedade **assigneePriority** em tarefas                                            |
| Modo de exibição de quadro com colunas para os destinatários (atribuídos ao quadro de tarefas)                            | Objeto [assignedToTaskBoardTaskFormat](plannerassignedtotaskboardtaskformat.md) |
| O modo de exibição de quadro com colunas para o andamento da tarefa na direção de conclusão (quadro de tarefa de andamento) | Objeto [progressTaskBoardTaskFormat](plannerprogresstaskboardtaskformat.md)     |
| Modo de exibição de quadro com colunas personalizadas de tarefas (quadro de tarefa do bucket):                              | Objeto [bucketTaskBoardTaskFormat](plannerbuckettaskboardtaskformat.md)         |

As colunas personalizadas no painel de tarefas do bucket são representadas pelos objetos [bucket](plannerbucket.md), e a sua ordem, pela propriedade **orderHint** no objeto.

Toda a ordem é controlada pelos princípios descritos em [Dicas de ordem do Planner](planner-order-hint-format.md).

## <a name="planner-resource-versioning"></a>Versão do recurso do Planner

O Planner cria versões de todos os recursos usando etags. Esses etags são devolvidos com a propriedade **@odata.etag** em cada recurso. As solicitações `PATCH` e `DELETE` requerem que a última etag conhecida pelo cliente seja especificada com um cabeçalho `If-Match`.
O Planner permite alterações em versões mais antigas de recursos, se a alteração pretendida não estiver em conflito com as alterações mais recentes aceitas pelo serviço do Planner no mesmo recurso. Os clientes podem identificar qual etag para o mesmo recurso é mais recente ao calcular qual valor de etag é maior em comparação com a cadeia de caracteres ordinal. Cada recurso tem uma etag única. Não há comparações entre os valores de etags de recursos diferentes, incluindo aqueles com relações de confinamento.
Espera-se que os aplicativos cliente tratem dos controles de versão relacionados aos [códigos de erro](/graph/errors) `409` e `412` lendo a versão mais recente do item e resolvendo as alterações conflitantes.

## <a name="common-planner-error-conditions"></a>Condições de erro comuns do Planner

Além dos [erros gerais](/graph/errors) que se aplicam ao Microsoft Graph, algumas condições de erro são específicas da API do Planner.

### <a name="400-bad-request"></a>400 Solicitação Incorreta

Em alguns cenários comuns, as solicitações `POST` e `PATCH` podem retornar um código de status 400. Estas são algumas das mais comuns:

* As propriedades Open Type não têm os tipos corretos, ou o tipo não foi especificado, ou não contêm qualquer propriedade. Por exemplo, as propriedades [plannerAssignments](plannerassignments.md) com valores complexos precisam declarar a propriedade **@odata.type** com valor `microsoft.graph.plannerAssignment`.
* Os valores da dica de ordem não têm o formato correto. Por exemplo, um valor de dica de ordem está sendo definido diretamente como o valor retornado ao cliente.
* Os dados são ilogicamente inconsistentes. Por exemplo, a data de início da tarefa é posterior à data de conclusão da tarefa.

### <a name="403-forbidden"></a>403 Proibido

Além dos erros gerais, a API do Planner também devolve esse `403` código de status quando um limite definido pelo serviço foi excedido. Se este for o caso, a propriedade **code** no tipo de recurso do erro indicará o tipo do limite excedido pela solicitação.
Os valores possíveis para os tipos de limite são:

| Valor                         | Descrição                                                                                                                                                                                              |
| :---------------------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| MaximumProjectsOwnedByUser    | Foi excedido o número máximo de planos contidos pelo limite do grupo. Este limite se aplica a planos contidos por um grupo com base na propriedade **contêiner** do recurso [plannerPlan](plannerplan.md).                                         |
| MaximumProjectsSharedWithUser | Foi excedido o número máximo de planos compartilhados com um limite de usuário.  Este limite se baseia na propriedade **sharedWith** no recurso [plannerPlanDetails](plannerplandetails.md).                   |
| MaximumTasksCreatedByUser     | Foi excedido o número máximo de tarefas criadas pelo limite do usuário. Este limite se baseia na propriedade **createdBy** no recurso [plannerTask](plannertask.md).                                    |
| MaximumTasksAssignedToUser    | Foi excedido o número máximo de tarefas atribuídas ao limite do usuário. Este limite se baseia na propriedade **tarefas** no recurso [plannerTask](plannertask.md).                                 |
| MaximumTasksInProject         | Foi excedido o número máximo de tarefas no limite de um plano. Este limite se baseia na propriedade **planId** no recurso [plannerTask](plannertask.md).                                               |
| MaximumActiveTasksInProject   | Foi excedido o número máximo de tarefas que não foram concluídas no limite de um plano. Este limite se baseia no **planId** e nas propriedades **percentComplete** e no recurso [plannerTask](plannertask.md). |
| MaximumBucketsInProject       | Foi excedido o número máximo de buckets no limite de um plano. Este limite se baseia na propriedade **planId** no recurso [plannerBucket](plannerbucket.md).                                         |
| MaximumUsersSharedWithProject | A propriedade **sharedWith** no recurso [plannerPlanDetails](plannerplandetails.md) contém demasiados valores.                                                                                          |
| MaximumReferencesOnTask       | A propriedade **referências** no recurso [plannerTaskDetails](plannertaskdetails.md) contém demasiados valores.                                                                                          |
| MaximumChecklistItemsOnTask   | A propriedade **lista de verificação** no recurso [plannerTaskDetails](plannertaskdetails.md) contém demasiados valores.                                                                                           |
| MaximumAssigneesInTasks       | A propriedade **tarefas** no recurso [plannerTask](plannertask.md) contém demasiados valores.                                                                                                       |
| MaximumPlannerPlans       | O grupo já contém um **plano**. Atualmente, os grupos só podem conter um **plano**. **Observação:** alguns aplicativos da Microsoft podem ultrapassar esse limite. Futuramente, essa funcionalidade será estendida para todos os aplicativos.                                                                                                      |

### <a name="412-precondition-failed"></a>412 Falha na Pré-condição 

Todas as APIs do Planner `POST`, `PATCH`, e `DELETE` solicitações exigem que o `If-Match` cabeçalho seja especificado com o último valor de etag conhecido do recurso que está sujeito à solicitação.
O código de status 412 também pode ser retornado se o valor da etag especificado na solicitação já não corresponder a uma versão do recurso no serviço. Nesse caso, os clientes devem ler o recurso novamente e obter uma nova etag.

## <a name="whats-new"></a>O que há de novo
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

