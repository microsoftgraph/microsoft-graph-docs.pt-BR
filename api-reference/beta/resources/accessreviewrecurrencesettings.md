---
title: Tipo de recurso accessReviewRecurrenceSettings
description: Especifica que a revisão de acesso recorre a intervalos regulares.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 208d3e8f8c73c8de98a34aadbd616dc9f268925c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136637"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a>Tipo de recurso accessReviewRecurrenceSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O tipo de recurso **accessReviewRecurrenceSettings** é usado no recurso [accessReviewSettings](accessreviewsettings.md) e especifica que a revisão de acesso recorre a intervalos regulares.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
| :------- | :--- | :---------- |
| recurrenceType | String | O intervalo de recorrência. Vaules possíveis: `onetime` `weekly` , , ou `monthly` `quarterly` `halfyearly` `annual` .                                                                   |
| recurrenceEndType | String | Como termina a recorrência. Valores possíveis: `never` `endBy` , , ou `occurrences` `recurrenceCount` . Se `never` for, não haverá fim explícito da série de recorrência. Se `endBy` for, a recorrência terminará em uma determinada data. Se `occurrences` for, a série terminará `recurrenceCount` após a conclusão das instâncias da revisão. |
| durationInDays | Int32 | A duração em dias para recorrência. |
| recurrenceCount | Int32 | A contagem de recorrências, se o valor de **recurrenceEndType** for , ou 0 caso `occurrences` contrário. |

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewRecurrenceSettings"
}-->
```json
{
  "recurrenceType": "string",
  "recurrenceEndType": "string",
  "durationInDays": 1024,
  "recurrenceCount": 1024
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "accessReviewRecurrenceSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
