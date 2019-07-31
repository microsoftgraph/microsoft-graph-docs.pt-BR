---
title: tipo de recurso teamMessagingSettings
description: Configurações para definir a mensagens e menções na equipe.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3a89ed35c820338cde7b3f22a7345c860b1a4427
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964526"
---
# <a name="teammessagingsettings-resource-type"></a>tipo de recurso teamMessagingSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Configurações para configurar mensagens e menção na [equipe](team.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowUserEditMessages|Booliano|Se definido como true, os usuários podem editar suas mensagens.|
|allowUserDeleteMessages|Booliano|Se definido como true, os usuários podem excluir suas mensagens.|
|allowOwnerDeleteMessages|Booliano|Se definido como true, os proprietários podem excluir qualquer mensagem.|
|allowTeamMentions|Booliano|Se for definido como true, @team mencionadas serão permitidas.|
|allowChannelMentions|Booliano|Se for definido como true, @channel mencionadas serão permitidas.|

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
<!--
{
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
