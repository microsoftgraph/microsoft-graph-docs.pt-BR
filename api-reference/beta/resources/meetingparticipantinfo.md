---
title: tipo de recurso meetingParticipantInfo
description: Informações sobre um participante de uma reunião.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3df338760bd1d2ff74cc79c706944c9b5fa7104d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342391"
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
