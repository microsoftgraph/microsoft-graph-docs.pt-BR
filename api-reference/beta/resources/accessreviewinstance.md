---
title: tipo de recurso accessReviewInstance
description: Representa uma recorrência de um `accessReviewScheduleDefinition` .
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 480774950e2257b7af099c02cbe7c6571c0ce4c6
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000780"
---
# <a name="accessreviewinstance-resource-type"></a>tipo de recurso accessReviewInstance

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma recorrência de análise do Azure AD [Access](accessreviewsv2-root.md) . Se o [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) pai for uma revisão de acesso recorrente, as instâncias representarão cada recorrência. Uma revisão que não recorrente terá exatamente uma instância. As instâncias também representam cada grupo único que está sendo revisado na definição de agendamento. Se uma definição de programação revisa vários grupos, cada grupo terá uma instância exclusiva para cada recorrência.

Cada **accessReviewInstance** contém uma lista de [decisões](accessreviewinstancedecisionitem.md) nas quais os revisores podem executar ações. Há uma decisão por identidade sendo revisada.

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:---------------|:--------|:----------|
|[Listar accessReviewInstances](../api/accessreviewinstance-list.md) | coleção [accessReviewInstance](accessreviewinstance.md) | Obtenha uma lista dos objetos [accessReviewInstance](../resources/accessreviewinstance.md) e suas propriedades. |
|[Obter accessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | Retorna accessReviewInstance para um accessReviewScheduleDefinition. Não inclui os accessReviewInstanceDecisionItem associados no objeto. |
|[Listar pendingAccessReviewInstances](../api/accessreviewinstance-pendingaccessreviewinstances.md) | coleção [accessReviewInstance](accessreviewinstance.md) . | Obter todos os recursos do accessReviewInstance pendentes atribuídos ao usuário de chamada. |
|[Enviar lembrete accessReviewInstance](../api/accessreviewinstance-sendreminder.md) | Nenhum. | Envie um lembrete para os revisores de um accessReviewInstance. |
|[Parar accessReviewInstance](../api/accessreviewinstance-stop.md) | Nenhum. | Interromper manualmente um accessReviewInstance. |
|[Aceitar recomendações](../api/accessreviewinstance-acceptrecommendations.md) | Nenhum. | Permite que o usuário de chamada aceite a recomendação de decisão para cada accessReviewInstanceDecisionItem não revisado que eles são o revisor para um accessReviewInstance específico. |
|[Aplicar decisões](../api/accessreviewinstance-applydecisions.md) | Nenhum. | Aplicar a decisão manualmente em um accessReviewInstance. |



## <a name="properties"></a>Propriedades
| Propriedade | Tipo | Descrição |
| :-------------------------| :---------------------------------- | :---------- |
| id | Cadeia de caracteres | Identificador exclusivo da instância. |
| displayName | Cadeia de caracteres | Nome do accessReviewScheduleDefinition pai. |
| startDateTime | DateTimeOffset | DateTime quando a instância de revisão está agendada para iniciar. Pode estar no futuro. |
| endDateTime | DateTimeOffset | DateTime quando a instância de revisão está agendada para terminar. |
| status | cadeia de caracteres | Especifica o status de um accessReview. Os Estados típicos incluem,,,,,, `Initializing` `NotStarted` `Starting` `InProgress` `Completing` `Completed` `AutoReviewing` e `AutoReviewed` .  Somente leitura.|
| escopo | [accessReviewScope](accessreviewscope.md) | Criado com base no **escopo** e no **InstanceEnumerationScope** no nível accessReviewScheduleDefinition. Define o escopo dos usuários revisados em um grupo. No caso de uma revisão de grupo único, o escopo definido no `accessReviewScheduleDefinition` nível se aplica a todas as instâncias. No caso de revisão de todos os grupos, o escopo pode ser diferente para cada grupo. Somente leitura.  | 
| correta | coleção [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) | Cada usuário revisado em um accessReviewInstance tem um item de decisão que representa se o acesso foi aprovado, negado ou ainda não revisado. |
| definir |[accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Há exatamente um accessReviewScheduleDefinition associado a cada instância. É a agenda pai para a instância, onde as instâncias são criadas para cada recorrência de uma definição de revisão e cada grupo selecionado para análise pela definição. |

## <a name="relationships"></a>Relações

| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
| `definition`               |[accessReviewScheduleDefinition](accessreviewscheduledefinition.md)          | Há exatamente um `accessReviewScheduleDefinition` associado a cada instância. É a agenda pai para a instância, onde as instâncias são criadas para cada recorrência de uma definição de revisão e cada grupo selecionado para análise pela definição. |
| `decisions`               |coleção [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md)        | Cada usuário revisado em um `accessReviewInstance` tem um item de decisão que representa se eles foram aprovados, negados ou ainda não revisados. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "baseType": "",
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
