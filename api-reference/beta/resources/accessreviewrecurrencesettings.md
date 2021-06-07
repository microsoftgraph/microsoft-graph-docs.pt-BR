---
title: Tipo de recurso accessReviewRecurrenceSettings
description: Especifica que a revisão de acesso se recorre a intervalos regulares.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: cb2a05589bfa92331a213a489bfb2a5129850065
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755655"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a>Tipo de recurso accessReviewRecurrenceSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

O tipo de recurso **accessReviewRecurrenceSettings** é usado no recurso [accessReviewSettings](accessreviewsettings.md) e especifica que a revisão de acesso se recorre a intervalos regulares.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
| :------- | :--- | :---------- |
| recurrenceType | Cadeia de caracteres | O intervalo de recorrência. Vaules possíveis: `onetime` , , , ou `weekly` `monthly` `quarterly` `halfyearly` `annual` .                                                                   |
| recurrenceEndType | Cadeia de caracteres | Como a recorrência termina. Valores possíveis: `never` `endBy` , , ou `occurrences` `recurrenceCount` . Se for `never` , não haverá fim explícito da série de recorrência. Se for `endBy` , a recorrência terminará em uma determinada data. Se for , a série terminará após a conclusão das `occurrences` `recurrenceCount` instâncias da revisão. |
| durationInDays | Int32 | A duração em dias para recorrência. |
| recurrenceCount | Int32 | A contagem de recorrências, se o valor de **recorrênciaEndType** for `occurrences` , ou de outra `0` forma. |

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
