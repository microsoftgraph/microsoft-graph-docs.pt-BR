---
title: Tipo de recurso meetingCapability
description: Contém os recursos de uma reunião
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d8e1d3985f95ecc28bd986218d7ff668f65b1db8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960401"
---
# <a name="meetingcapability-resource-type"></a>Tipo de recurso meetingCapability

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém os recursos de uma reunião

## <a name="properties"></a>Propriedades

| Propriedade                          | Tipo    | Descrição                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| allowAnonymousUsersToDialOut      | Booliano | Indica se o discagem de usuários anônimos é permitido em uma reunião. |
| allowAnonymousUsersToStartMeeting | Booliano | Indica se os usuários anônimos têm permissão para iniciar uma reunião.  |
| autoAdmittedUsers                 | autoAdmittedUsersType  | Os valores possíveis são: `everyoneInCompany` e `everyone`.              |

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


