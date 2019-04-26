---
title: Tipo de recurso meetingTimeSuggestionsResult
description: Uma coleção de sugestões de reunião, se houver alguma, e a razão se não houver.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 1e3fb99e7675544f39b359abd226875a7721e287
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342307"
---
# <a name="meetingtimesuggestionsresult-resource-type"></a>Tipo de recurso meetingTimeSuggestionsResult

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Uma coleção de sugestões de reunião, se houver alguma, e a razão se não houver.

A seguir estão os possíveis motivos que [findMeetingTimes](../api/user-findmeetingtimes.md) não retorna as sugestões de reunião.

|**valor de emptySuggestionsReason**|**Motivos**|
|:-----|:-----|
| attendeesUnavailable | A disponibilidade de todos os participantes é conhecida, mas não há participantes suficientes disponíveis para alcançar o limite de [confiança da reunião](../api/user-findmeetingtimes.md#the-confidence-of-a-meeting-suggestion) , que é de 50% por padrão, para qualquer período de tempo.|
| attendeesUnavailableOrUnknown | Alguns ou todos os participantes têm disponibilidade desconhecida, fazendo com que a confiança na reunião caia para abaixo o limite definido, que é de 50% por padrão. A disponibilidade do participante poderá se tornar desconhecida se ele não for da organização ou se houver um erro ao obter informações sobre a disponibilidade.|
| locationsUnavailable | A **** propriedade IsRequired do parâmetro **locationConstraint** é especificada como true e, ainda, não há locais disponíveis nos intervalos de tempo calculados. |
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
|emptySuggestionsReason|Cadeia de caracteres|Um motivo para não retornar qualquer sugestão de reunião. Os valores possíveis são: `attendeesUnavailable`, `attendeesUnavailableOrUnknown`, `locationsUnavailable`, `organizerUnavailable` ou `unknown`. Esta propriedade é uma cadeia de caracteres vazia se a propriedade **meetingTimeSuggestions** inclui qualquer sugestão de reunião.|
|meetingTimeSuggestions|Coleção [meetingTimeSuggestion](meetingtimesuggestion.md)|Uma matriz de sugestões de reunião.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingTimeSuggestionsResult resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
