---
title: tipo de recurso teamMemberSettings
description: Configurações para configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots na equipe.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: f77bc80a5723e3e00675aeaab05f2dd7ea180f76
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519936"
---
# <a name="teammembersettings-resource-type"></a>tipo de recurso teamMemberSettings

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Configurações para configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots, na [equipe](team.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|Boolean|Se definido como true, os membros podem adicionar e atualizar qualquer canal.|
|allowCreatePrivateChannels|Boolean|Se definido como true, os membros podem adicionar e atualizar canais privados.|
|allowDeleteChannels|Boolean|Se definido como true, os membros podem excluir canais.|
|allowAddRemoveApps|Boolean|Se definido como true, os membros podem adicionar e remover aplicativos.|
|allowCreateUpdateRemoveTabs|Boolean|Se definido como true, os membros podem adicionar, atualizar e remover guias. |
|allowCreateUpdateRemoveConnectors|Boolean|Se definido como true, os membros podem adicionar, atualizar e remover conectores.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMemberSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowCreatePrivateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
