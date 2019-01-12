---
title: tipo de recurso de meetingCapability
description: Contém os recursos de uma reunião
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 342d264c1f4c670d159c15558c78cc896d4a9487
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931360"
---
# <a name="meetingcapability-resource-type"></a>tipo de recurso de meetingCapability

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Contém os recursos de uma reunião

## <a name="properties"></a>Propriedades

| Propriedade                          | Tipo    | Descrição                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| allowAnonymousUsersToDialOut      | Booliano | Indica se os usuários anônimos discagem é permitida em uma reunião. |
| allowAnonymousUsersToStartMeeting | Booliano | Indica se os usuários anônimos poderão iniciar uma reunião.  |
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
<!-- {
  "type": "#page.annotation",
  "description": "meetingCapability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
