---
title: Tipo de recurso timeCardEvent
description: Representa um evento de cartão de ponto específico.
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a8be7d000b3d55368f7378e9b993b5015b7ef632
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786361"
---
# <a name="timecardevent-resource-type"></a>Tipo de recurso timeCardEvent

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um evento [timeCard](timecard.md) específico.

## <a name="properties"></a>Propriedades
|Propriedade               |Tipo           |Descrição                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| dateTime                  |`Edm.dateTimeOffset`  |A hora em que a entrada é gravada. |
| atApprovedLocation |`Edm.boolean `  |Indica se a entrada foi registrada no local aprovado. |
| notes                 |[itemBody](itembody.md)  | Observações sobre **o timeCardEvent**.|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeCardEvent"
}-->
```json
{
   "atApprovedLocation":true,
   "notes":{ "@odata.type":"microsoft.graph.itemBody" }
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeCardEvent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
