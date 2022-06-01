---
title: Tipo de recurso accessReviewRecurrenceSettings (preterido)
description: Especifica que a revisão de acesso se repetirá em intervalos regulares.
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 9fa6fb47c541094c85778621289d1abb6d71f727
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65821208"
---
# <a name="accessreviewrecurrencesettings-resource-type-deprecated"></a>Tipo de recurso accessReviewRecurrenceSettings (preterido)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

O **tipo de recurso accessReviewRecurrenceSettings** é usado no recurso [accessReviewSettings](accessreviewsettings.md) e especifica que a revisão de acesso se repetirá em intervalos regulares.

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
| :------- | :--- | :---------- |
| recurrenceType | Cadeia de caracteres | O intervalo de recorrência. Possíveis vaules: `onetime`, `weekly`, `monthly`, `quarterly`, `halfyearly` ou `annual`.                                                                   |
| recurrenceEndType | String | Como a recorrência termina. Valores possíveis: `never`, `endBy`, `occurrences`ou `recurrenceCount`. Se for `never`, não haverá nenhum fim explícito da série de recorrência. Se for, `endBy`a recorrência terminará em uma determinada data. Se for, `occurrences`a série terminará depois que `recurrenceCount` as instâncias da revisão forem concluídas. |
| durationInDays | Int32 | A duração em dias para recorrência. |
| recurrenceCount | Int32 | A contagem de recorrências, se o valor de **recurrenceEndType** for `occurrences`ou não `0` . |

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
