---
title: Tipo de recurso attendeeAvailability
description: O tipo e a disponibilidade dos participantes.
localization_priority: Normal
ms.openlocfilehash: a00fe38e678c6a51cd252b823a7d2651e531d20a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820465"
---
# <a name="attendeeavailability-resource-type"></a>Tipo de recurso attendeeAvailability

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O tipo e a disponibilidade dos participantes.

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
|attendee|[AttendeeBase](attendeebase.md)|O tipo de participante, ou seja, se é um recurso ou uma pessoa e, no caso de uma pessoa, se é obrigatório ou opcional.|
|availability|Cadeia de caracteres| O status de disponibilidade do participante. Os possíveis valores são: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeAvailability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
