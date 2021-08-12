---
title: Tipo de recurso accessReviewInstance
description: Representa uma recorrência de um `accessReviewScheduleDefinition` .
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: c2790b6c7cace35decb969e720fa2175f6333f8c4a594d02137c28aaeb47b94c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54212260"
---
# <a name="accessreviewinstance-resource-type"></a>Tipo de recurso accessReviewInstance

Namespace: microsoft.graph

Representa uma recorrência de revisão de acesso [do](accessreviewsv2-root.md) Azure AD. Gerado pelo sistema com base no [access paiReviewScheduleDefinition](accessreviewscheduledefinition.md). Todas as propriedades são somente leitura.

Se a instância faz parte de uma revisão de acesso recorrente, as instâncias representam cada recorrência. Uma revisão que não se recorre terá exatamente uma instância. As instâncias também representam cada recurso exclusivo que está sendo revisado na definição de agendamento. Se uma definição de agenda analisar vários recursos, cada recurso terá uma instância exclusiva para cada recorrência.

Cada **accessReviewInstance** contém uma lista de [decisões](accessreviewinstancedecisionitem.md) que os revisores podem tomar medidas. Há uma decisão por identidade sendo revisada.

Herda da [entidade](../resources/entity.md).

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar accessReviewInstances](../api/accessreviewinstance-list.md)|[Coleção accessReviewInstance](../resources/accessreviewinstance.md)|Obter uma lista dos [objetos accessReviewInstance](../resources/accessreviewinstance.md) e suas propriedades.|
|[Obter accessReviewInstance](../api/accessreviewinstance-get.md)|[accessReviewInstance](../resources/accessreviewinstance.md)|Leia as propriedades e as relações de um [objeto accessReviewInstance.](../resources/accessreviewinstance.md)|
|[stop](../api/accessreviewinstance-stop.md)|None|Pare manualmente um accessReviewInstance.|
|[sendReminder](../api/accessreviewinstance-sendreminder.md)|None|Envie um lembrete aos revisores de um accessReviewInstance.|
|[resetDecisions](../api/accessreviewinstance-resetdecisions.md)|None|Redefine todos os itens de decisão em uma instância para `notReviewed`|
|[applyDecisions](../api/accessreviewinstance-applydecisions.md)|None|Aplicar manualmente a decisão em um accessReviewInstance.|
|[acceptRecommendations](../api/accessreviewinstance-acceptrecommendations.md)|None| Permite que o usuário de chamada aceite a recomendação de decisão para cada acesso NotReviewInstanceDecisionItem em que ele é o revisor para um accessReviewInstance específico.|
|[batchRecordDecisions](../api/accessreviewinstance-batchrecorddecisions.md)|None|Revise lotes de entidades ou recursos em uma chamada.|
|[filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[Coleção accessReviewInstance](../resources/accessreviewinstance.md)|Retorna todos os objetos de instância em uma definição para a qual o usuário de chamada é o revistor.|
|[Listar decisões](../api/accessreviewinstance-list-decisions.md)|[Coleção accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Obter os recursos accessReviewInstanceDecisionItem da propriedade de navegação de decisões.|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
| id | Cadeia de caracteres | Identificador exclusivo da instância. Herdado da [entidade](../resources/entity.md). Oferece suporte para `$select`. Somente leitura.|
| startDateTime | DateTimeOffset | DateTime quando a instância de revisão está agendada para começar. Pode ser no futuro. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Oferece suporte para `$select`. Somente leitura. |
| endDateTime | DateTimeOffset | DateTime quando a instância de revisão está agendada para terminar. O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Oferece suporte para `$select`. Somente leitura.|
| status | Cadeia de caracteres | Especifica o status de um accessReview. Valores possíveis: `Initializing` , , , , , , e `NotStarted` `Starting` `InProgress` `Completing` `Completed` `AutoReviewing` `AutoReviewed` . Suporta `$select` `$orderby` , e ( `$filter` `eq` somente). Somente leitura.|
| escopo | [accessReviewScope](accessreviewscope.md) | Criado com base **no escopo** e **instanceEnumerationScope** no nível accessReviewScheduleDefinition. Define o escopo dos usuários revisados em um grupo. Suporta `$select` e `$filter` ( `contains` somente). Somente leitura. |

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|decisions|[Coleção accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Cada entidade revisada em um tem um item de decisão que representa se foram `accessReviewInstance` aprovados, negados ou ainda não revisados.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInstance",
  "id": "String (identifier)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "status": "String",
  "scope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  }
}
```
