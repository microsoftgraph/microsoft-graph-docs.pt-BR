---
title: Tipo de recurso accessReviewInstance
description: Representa uma recorrência de um `accessReviewScheduleDefinition` .
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f77e5ae6d16b96fff2586b5b2bd920d01737196d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59025668"
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
| endDateTime | DateTimeOffset | DateTime quando a instância de revisão está agendada para terminar. O tipo DatetimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Oferece suporte para `$select`. Somente leitura.|
| fallbackReviewers   |[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Essa coleção de escopos do revistor é usada para definir a lista de revisadores de fallback. Esses revisadores de fallback serão notificados para tomar medidas se nenhum usuário for encontrado na lista de revisadores especificados. Isso pode ocorrer quando o proprietário do grupo é especificado como o revistor, mas o proprietário do grupo não existe, ou o gerente é especificado como revistor, mas o gerente de um usuário não existe. Suporta o `$select`.|
| id | String | Identificador exclusivo da instância. Herdado da [entidade](../resources/entity.md). Oferece suporte para `$select`. Somente leitura.|
| escopo | [accessReviewScope](accessreviewscope.md) | Criado com base **no escopo** e **instanceEnumerationScope** no nível accessReviewScheduleDefinition. Define o escopo dos usuários revisados em um grupo. Suporta `$select` e `$filter` ( `contains` somente). Somente leitura. |
| startDateTime | DateTimeOffset | DateTime quando a instância de revisão está agendada para começar. Pode ser no futuro. O tipo DateTimeOffset representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Oferece suporte para `$select`. Somente leitura. |
| status | String | Especifica o status de um accessReview. Valores possíveis: `Initializing` , , , , , , e `NotStarted` `Starting` `InProgress` `Completing` `Completed` `AutoReviewing` `AutoReviewed` . Suporta `$select` `$orderby` , e ( `$filter` `eq` somente). Somente leitura.|
| revisadores   |[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)| Essa coleção de escopos de revisão de acesso é usada para definir quem são os revisadores. Suporta o `$select`. Para exemplos de opções para atribuir revisadores, consulte Atribuir revisadores à sua definição de revisão de acesso [usando a API do Microsoft Graph](/graph/accessreviews-scope-concept).|


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
  },
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ],
  "fallbackReviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ]
}
```
