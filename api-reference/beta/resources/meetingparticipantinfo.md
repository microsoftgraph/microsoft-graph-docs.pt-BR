---
title: tipo de recurso meetingParticipantInfo
description: Informações sobre um participante de uma reunião.
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2775dd3af7940f9022b9e7090125ed52fce397d6
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006631"
---
# <a name="meetingparticipantinfo-resource-type"></a>tipo de recurso meetingParticipantInfo

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Informações sobre um participante de uma reunião.

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                          | Descrição                              |
|:---------------|:------------------------------|:-----------------------------------------|
| ladrões       | [identitySet](identityset.md) | Informações de identidade do participante. |
| UPN            | String                        | Nome principal do usuário do participante.  |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipantInfo"
}-->
```json
{
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "upn": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
