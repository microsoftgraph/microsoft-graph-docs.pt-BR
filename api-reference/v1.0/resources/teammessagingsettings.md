---
title: Tipo de recurso teamMessagingSettings
description: Configurações para definir a mensagens e menções na equipe.
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 08af21e988862a4d6b459953e6d1a1fd5554da36
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59049484"
---
# <a name="teammessagingsettings-resource-type"></a>Tipo de recurso teamMessagingSettings

Namespace: microsoft.graph



Configurações configurar mensagens e menções na [equipe](team.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowUserEditMessages|Boolean|Se definido como true, os usuários podem editar suas mensagens.|
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

