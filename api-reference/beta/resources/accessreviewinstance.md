---
title: Tipo de recurso accessReviewInstance
description: Representa uma recorrência de um `accessReviewScheduleDefinition` .
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0f480b870af2fd4717ff1341a1ab66b73301fc7f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158531"
---
# <a name="accessreviewinstance-resource-type"></a>Tipo de recurso accessReviewInstance

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma recorrência de revisão de acesso [do](accessreviewsv2-root.md) Azure AD. Se o [accessReviewScheduleDefinition pai](accessreviewscheduledefinition.md) for uma revisão de acesso recorrente, as instâncias representarão cada recorrência. Uma revisão que não recorre terá exatamente uma instância. As instâncias também representam cada grupo exclusivo que está sendo revisado na definição de agendamento. Se uma definição de agenda analisar vários grupos, cada grupo terá uma instância exclusiva para cada recorrência.

Cada **accessReviewInstance** contém uma lista de [decisões que](accessreviewinstancedecisionitem.md) os revisores podem tomar medidas. Há uma decisão por identidade sendo revisada.

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Listar accessReviewInstances](../api/accessreviewinstance-list.md) | [Coleção accessReviewInstance](accessreviewinstance.md) | Obter uma lista dos [objetos accessReviewInstance](../resources/accessreviewinstance.md) e suas propriedades. |
|[Acessar AccessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | Retorna accessReviewInstance para um accessReviewScheduleDefinition. Não inclui accessReviewInstanceDecisionItem associado no objeto. |
|[Listar pendingAccessReviewInstances](../api/accessreviewinstance-pendingaccessreviewinstances.md) | [Coleção accessReviewInstance.](accessreviewinstance.md) | Obter todos os recursos pendentes accessReviewInstance atribuídos ao usuário de chamada. |
|[Enviar lembrete accessReviewInstance](../api/accessreviewinstance-sendreminder.md) | Nenhum. | Envie um lembrete aos revisores de um accessReviewInstance. |
|[Parar accessReviewInstance](../api/accessreviewinstance-stop.md) | Nenhum. | Pare manualmente um accessReviewInstance. |
|[Aceitar recomendações](../api/accessreviewinstance-acceptrecommendations.md) | Nenhum. | Permite que o usuário de chamada aceite a recomendação de decisão para cada NotReviewInstanceDecisionItem em que ele é o revisor para um accessReviewInstance específico. |
|[Aplicar decisões](../api/accessreviewinstance-applydecisions.md) | Nenhum. | Aplique manualmente a decisão em um accessReviewInstance. |



## <a name="properties"></a>Propriedades
| Propriedade | Tipo | Descrição |
| :-------------------------| :---------------------------------- | :---------- |
| id | String | Identificador exclusivo da instância. |
| displayName | String | Nome do accessReviewScheduleDefinition pai. |
| startDateTime | DateTimeOffset | DateTime quando a instância de revisão está agendada para iniciar. Pode ser no futuro. |
| endDateTime | DateTimeOffset | DateTime quando a instância de revisão está agendada para terminar. |
| status | cadeia de caracteres | Especifica o status de um accessReview. Os estados típicos `Initializing` `NotStarted` incluem , `Starting` , , , e `InProgress` `Completing` `Completed` `AutoReviewing` `AutoReviewed` .  Somente leitura.|
| escopo | [accessReviewScope](accessreviewscope.md) | Criado com base **no escopo** **e instanceEnumerationScope** no nível accessReviewScheduleDefinition. Define o escopo dos usuários analisados em um grupo. No caso de uma revisão de grupo único, o escopo definido no nível se aplica a `accessReviewScheduleDefinition` todas as instâncias. No caso de todas as revisões de grupos, o escopo pode ser diferente para cada grupo. Somente leitura.  | 
| decisões | [Coleção accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) | Cada usuário revisado em um accessReviewInstance tem um item de decisão representando se seu acesso foi aprovado, negado ou ainda não revisado. |
| definição |[accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Há exatamente um accessReviewScheduleDefinition associado a cada instância. É a agenda pai da instância, onde as instâncias são criadas para cada recorrência de uma definição de revisão e cada grupo selecionado para revisar pela definição. |

## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `definition`               |[accessReviewScheduleDefinition](accessreviewscheduledefinition.md)          | Há exatamente um `accessReviewScheduleDefinition` associado a cada instância. É a agenda pai da instância, onde as instâncias são criadas para cada recorrência de uma definição de revisão e cada grupo selecionado para revisar pela definição. |
| `decisions`               |[Coleção accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md)        | Cada usuário revisado em um tem um item de decisão representando se eles `accessReviewInstance` foram aprovados, negados ou ainda não revisados. |

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
