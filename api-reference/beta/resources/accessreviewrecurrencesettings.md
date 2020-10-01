---
title: tipo de recurso accessReviewRecurrenceSettings
description: Especifica que a revisão do Access se repete em intervalos regulares.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3ca66a818059efac84903f763e6be3c8a3b5c05a
ms.sourcegitcommit: 8ed1280dc0a4f04075d32feac00003a30a2ad9a8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/01/2020
ms.locfileid: "48330162"
---
# <a name="accessreviewrecurrencesettings-resource-type"></a>tipo de recurso accessReviewRecurrenceSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O tipo de recurso **accessReviewRecurrenceSettings** é usado no recurso [accessReviewSettings](accessreviewsettings.md) e especifica que a revisão de acesso se repete em intervalos regulares.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
| :------- | :--- | :---------- |
| recurrenceType | Cadeia de caracteres | O intervalo de recorrência. Possível vaules: `onetime` , `weekly` , `monthly` , `quarterly` `halfyearly` ou `annual` .                                                                   |
| recurrenceEndType | Cadeia de caracteres | Como a recorrência termina. Valores possíveis: `never` , `endBy` , `occurrences` ou `recurrenceCount` . Se for `never` , não haverá uma extremidade explícita da série de recorrência. Se for `endBy` , a recorrência terminará em uma determinada data. Se for `occurrences` , a série terminará após a `recurrenceCount` conclusão das instâncias da revisão. |
| durationInDays | Int32 | A duração em dias da recorrência. |
| recurrenceCount | Int32 | A contagem de recorrências, se o valor de **recurrenceEndType** for `occurrences` , ou 0 caso contrário. |

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