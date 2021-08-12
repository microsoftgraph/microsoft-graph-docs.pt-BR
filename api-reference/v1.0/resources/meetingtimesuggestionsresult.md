---
title: Tipo de recurso meetingTimeSuggestionsResult
description: Uma coleção de sugestões de reunião, se houver alguma, ou se não houver motivo.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 441ba167cdc90128ec63403bfe389de68de6c56d1c506c9479e5c9ffa433a64c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54230435"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a>Tipo de recurso meetingTimeSuggestionsResult

Namespace: microsoft.graph

Uma coleção de sugestões de reunião, se houver alguma, ou se não houver motivo.

A seguir estão os possíveis motivos que [findMeetingTimes](../api/user-findmeetingtimes.md) não retorna as sugestões de reunião.

|**valor de emptySuggestionsReason**|**Motivos**|
|:-----|:-----|
| attendeesUnavailable | Toda a disponibilidade dos participantes é conhecida, mas não há participantes [](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) suficientes disponíveis para alcançar o limite de confiança da reunião, que é de 50% por padrão, para qualquer período de tempo.|
| attendeesUnavailableOrUnknown | Alguns ou todos os participantes têm disponibilidade desconhecida, fazendo com que a confiança na reunião caia para abaixo o limite definido, que é de 50% por padrão. A disponibilidade do participante poderá se tornar desconhecida se ele não for da organização ou se houver um erro ao obter informações sobre a disponibilidade.|
| locationsUnavailable | A propriedade **isRequired** do parâmetro [locationConstraint](locationconstraint.md) é especificada como obrigatória, e ainda não existem locais disponíveis nos intervalos de tempo calculados. |
| organizerUnavailable | O parâmetro **isOrganizerOptional** é falso, e o organizador não está disponível durante a janela de tempo solicitada. |
| desconhecido | O motivo para não retornar qualquer sugestão de reunião não é conhecido.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingTimeSuggestionsResult"
}-->

```json
{
  "emptySuggestionsReason": "String",
  "meetingTimeSuggestions": [{"@odata.type": "microsoft.graph.meetingTimeSuggestion"}]
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|emptySuggestionsReason|Cadeia de caracteres|Um motivo para não retornar qualquer sugestão de reunião. Os valores possíveis são: `attendeesUnavailable` , , , , ou `attendeesUnavailableOrUnknown` `locationsUnavailable` `organizerUnavailable` `unknown` . Essa propriedade será uma cadeia de caracteres vazia se a **propriedade meetingTimeSuggestions** incluir sugestões de reunião.|
|meetingTimeSuggestions|Coleção [meetingTimeSuggestion](meetingtimesuggestion.md)|Uma matriz de sugestões de reunião.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

