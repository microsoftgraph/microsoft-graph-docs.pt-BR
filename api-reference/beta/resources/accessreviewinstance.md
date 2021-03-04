---
title: Tipo de recurso accessReviewInstance
description: Representa uma recorrência de um `accessReviewScheduleDefinition` .
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a0003ab8a79372a4dfefea1a62120ea8e40fa2c1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443192"
---
# <a name="accessreviewinstance-resource-type"></a>Tipo de recurso accessReviewInstance

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Representa uma recorrência de revisão de acesso [do](accessreviewsv2-root.md) Azure AD. Se o [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) pai for uma revisão de acesso recorrente, as instâncias representarão cada recorrência. Uma revisão que não se recorre terá exatamente uma instância. As instâncias também representam cada grupo exclusivo que está sendo revisado na definição de agendamento. Se uma definição de agenda analisar vários grupos, cada grupo terá uma instância exclusiva para cada recorrência.

Cada **accessReviewInstance** contém uma lista de [decisões](accessreviewinstancedecisionitem.md) que os revisores podem tomar medidas. Há uma decisão por identidade sendo revisada.

## <a name="methods"></a>Methods

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Listar accessReviewInstances](../api/accessreviewinstance-list.md) | [Coleção accessReviewInstance](accessreviewinstance.md) | Obter uma lista dos [objetos accessReviewInstance](../resources/accessreviewinstance.md) e suas propriedades. |
|[Obter accessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | Retorna accessReviewInstance para um accessReviewScheduleDefinition. Não inclui accessReviewInstanceDecisionItem associado no objeto. |
|[Listar pendingAccessReviewInstances](../api/accessreviewinstance-pendingaccessreviewinstances.md) | [Coleção accessReviewInstance.](accessreviewinstance.md) | Obter todos os recursos de accessReviewInstance pendentes atribuídos ao usuário de chamada. |
|[Enviar lembrete accessReviewInstance](../api/accessreviewinstance-sendreminder.md) | Nenhum. | Envie um lembrete aos revisores de um accessReviewInstance. |
|[Parar accessReviewInstance](../api/accessreviewinstance-stop.md) | Nenhum. | Pare manualmente um accessReviewInstance. |
|[Aceitar recomendações](../api/accessreviewinstance-acceptrecommendations.md) | Nenhum. | Permite que o usuário de chamada aceite a recomendação de decisão para cada acesso NotReviewInstanceDecisionItem em que ele é o revisor para um accessReviewInstance específico. |
|[Aplicar decisões](../api/accessreviewinstance-applydecisions.md) | Nenhum. | Aplicar manualmente a decisão em um accessReviewInstance. |



## <a name="properties"></a>Propriedades
| Propriedade | Tipo | Descrição |
| :-------------------------| :---------------------------------- | :---------- |
| id | String | Identificador exclusivo da instância. |
| displayName | String | Nome do access paiReviewScheduleDefinition. |
| startDateTime | DateTimeOffset | DateTime quando a instância de revisão está agendada para começar. Pode ser no futuro. |
| endDateTime | DateTimeOffset | DateTime quando a instância de revisão está agendada para terminar. |
| status | cadeia de caracteres | Especifica o status de um accessReview. Os estados típicos `Initializing` `NotStarted` incluem , `Starting` , , , , , e `InProgress` `Completing` `Completed` `AutoReviewing` `AutoReviewed` .  Somente leitura.|
| escopo | [accessReviewScope](accessreviewscope.md) | Criado com base **no escopo** e **instanceEnumerationScope** no nível accessReviewScheduleDefinition. Define o escopo dos usuários revisados em um grupo. No caso de uma revisão de grupo único, o escopo definido no `accessReviewScheduleDefinition` nível se aplica a todas as instâncias. No caso da revisão de todos os grupos, o escopo pode ser diferente para cada grupo. Somente leitura.  | 
| decisions | [Coleção accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) | Cada usuário revisado em um accessReviewInstance tem um item de decisão que representa se seu acesso foi aprovado, negado ou ainda não revisado. |
| definition |[accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Há exatamente um accessReviewScheduleDefinition associado a cada instância. É a agenda pai da instância, onde as instâncias são criadas para cada recorrência de uma definição de revisão e cada grupo selecionado para revisar pela definição. |

## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `definition`               |[accessReviewScheduleDefinition](accessreviewscheduledefinition.md)          | Há exatamente um `accessReviewScheduleDefinition` associado a cada instância. É a agenda pai da instância, onde as instâncias são criadas para cada recorrência de uma definição de revisão e cada grupo selecionado para revisar pela definição. |
| `decisions`               |[Coleção accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md)        | Cada usuário revisado em um tem um item de decisão representando se eles foram `accessReviewInstance` aprovados, negados ou ainda não revisados. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "openType": false
}
-->

```json
{
 "@odata.type": "#microsoft.graph.accessReviewInstance",
 "id": "string (identifier)",
 "displayName": "string",
 "startDateTime": "string (timestamp)",
 "endDateTime": "string (timestamp)",
 "status": "string",
 "scope": {
    "@odata.type": "microsoft.graph.accessReviewScope"
  }
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewInstance resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
