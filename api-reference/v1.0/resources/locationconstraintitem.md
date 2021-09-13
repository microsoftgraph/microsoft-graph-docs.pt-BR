---
title: Tipo de recurso locationConstraintItem
description: As condições indicadas por um cliente para o local de uma reunião.
ms.localizationpriority: medium
author: harini84
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f9f4e550c1378cd40acf99bd93c2a24f847a9ca0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134672"
---
# <a name="locationconstraintitem-resource-type"></a>Tipo de recurso locationConstraintItem

Namespace: microsoft.graph

As condições indicadas por um cliente para o local de uma reunião.

Derivado de [location](location.md).

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.location",
  "@odata.type": "microsoft.graph.locationConstraintItem"
}-->

```json
{
  "resolveAvailability": true,
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "displayName": "string",
  "locationEmailAddress": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| address | [physicalAddress](physicaladdress.md) |O endereço físico do local. |
| displayName  | Cadeia de caracteres | O nome associado ao local.                       |
| locationEmailAddress | String | O endereço de email opcional do local. |
| resolveAvailability | Booliano | Se definido como true e o recurso especificado está ocupado, [findMeetingTimes](../api/user-findmeetingtimes.md) procura outro recurso livre. Se definido como false e o recurso especificado está ocupado, **findMeetingTimes** retorna o recurso melhor classificado no cache do usuário sem verificar se ele está livre. O padrão é true. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "locationConstraintItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

