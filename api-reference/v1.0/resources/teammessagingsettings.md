---
title: Tipo de recurso teamMessagingSettings
description: Configurações para definir a mensagens e menções na equipe.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9818e161e21f78a83023ead66d7b790eadd01bb2737942a383665338d0ec73c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129957"
---
# <a name="teammessagingsettings-resource-type"></a>Tipo de recurso teamMessagingSettings

Namespace: microsoft.graph



Configurações configurar mensagens e menções na [equipe](team.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowUserEditMessages|Booliano|Se definido como true, os usuários podem editar suas mensagens.|
|allowUserDeleteMessages|Booliano|Se for definido como true, os usuários poderão excluir suas mensagens.|
|allowOwnerDeleteMessages|Booliano|Se definido como true, os proprietários poderão excluir qualquer mensagem.|
|allowTeamMentions|Booliano|Se definido como true, @team as menções são permitidas.|
|allowChannelMentions|Booliano|Se definido como true, @channel as menções são permitidas.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMessagingSettings"
}-->

```json
{
  "allowUserEditMessages": true,
  "allowUserDeleteMessages": true,
  "allowOwnerDeleteMessages": true,
  "allowTeamMentions": true,
  "allowChannelMentions": true    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

