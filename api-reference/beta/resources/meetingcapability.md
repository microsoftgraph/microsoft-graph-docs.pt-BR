---
title: tipo de recurso meetingCapability
description: Contém os recursos de uma reunião
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2b891a9e6d0eb90a527c79528e9fd595c2f8ca5b
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913622"
---
# <a name="meetingcapability-resource-type"></a>tipo de recurso meetingCapability

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém os recursos de uma reunião

## <a name="properties"></a>Propriedades

| Propriedade                          | Tipo    | Descrição                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| allowAnonymousUsersToDialOut      | Booliano | Indica se os usuários anônimos de discagem são permitidos em uma reunião. |
| allowAnonymousUsersToStartMeeting | Booliano | Indica se os usuários anônimos podem iniciar uma reunião.  |
| autoAdmittedUsers                 | String  | Os valores possíveis são: `everyoneInCompany` e `everyone`.              |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingCapability"
}-->
```json
{
  "allowAnonymousUsersToDialOut": true,
  "allowAnonymousUsersToStartMeeting": true,
  "autoAdmittedUsers": "everyoneInCompany | everyone"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingCapability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
