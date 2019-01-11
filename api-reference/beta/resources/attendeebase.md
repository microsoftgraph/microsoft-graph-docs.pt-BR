---
title: Tipo de recurso attendeeBase
description: O tipo de participante.
localization_priority: Normal
ms.openlocfilehash: b30e054e6d89765d280340b31355403739381c2a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844976"
---
# <a name="attendeebase-resource-type"></a>Tipo de recurso attendeeBase

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O tipo de participante.

Derivado do [destinatário](recipient.md).

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendeeBase"
}-->

```json
{
  "type": "String",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|type|Cadeia de caracteres| O tipo de participante. Os valores possíveis são: `required`, `optional`, `resource`. Atualmente, se o participante é uma pessoa, [findMeetingTimes](../api/user-findmeetingtimes.md) sempre considera que a pessoa é do tipo `Required`.|
|emailAddress|[emailAddress](emailaddress.md)|Inclui o nome e endereço SMTP do participante.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "attendeeBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
