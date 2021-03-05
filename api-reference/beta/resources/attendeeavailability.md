---
title: Tipo de recurso attendeeAvailability
description: A disponibilidade de um participante.
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 9cfdc6b1f944457d24f1b569aa3d6263e6375aa8
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50473564"
---
# <a name="attendeeavailability-resource-type"></a>Tipo de recurso attendeeAvailability

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A disponibilidade de um participante.

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeAvailability"
}-->

```json
{
  "attendee": {"@odata.type": "microsoft.graph.attendeeBase"},
  "availability": "String"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|attendee|[attendeeBase](attendeebase.md)|O endereço de email e o tipo de participante - se é uma pessoa ou um recurso e se é obrigatório ou opcional se for uma pessoa.|
|availability|freeBusyStatus| O status de disponibilidade do participante. Os possíveis valores são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


