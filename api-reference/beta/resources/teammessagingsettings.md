---
title: tipo de recurso teamMessagingSettings
description: Configurações para definir a mensagens e menções na equipe.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 48d9281a032bebd9d65936cbf9effd78416ffc7d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341438"
---
# <a name="teammessagingsettings-resource-type"></a>tipo de recurso teamMessagingSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Configurações para configurar mensagens e menção na [equipe](team.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowUserEditMessages|Boolean|Se definido como true, os usuários podem editar suas mensagens.|
|allowUserDeleteMessages|Boolean|Se definido como true, os usuários podem excluir suas mensagens.|
|allowOwnerDeleteMessages|Boolean|Se definido como true, os proprietários podem excluir qualquer mensagem.|
|allowTeamMentions|Boolean|Se for definido como true, @team mencionadas serão permitidas.|
|allowChannelMentions|Boolean|Se for definido como true, @channel mencionadas serão permitidas.|

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
