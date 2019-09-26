---
title: tipo de recurso teamMemberSettings
description: Configurações para configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots na equipe.
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8967eb083ad2bd413277c42b688c2d0c48d8244b
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37196256"
---
# <a name="teammembersettings-resource-type"></a>tipo de recurso teamMemberSettings

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Configurações para configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots, na [equipe](team.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|Booliano|Se definido como true, os membros podem adicionar e atualizar qualquer canal.|
|allowCreatePrivateChannels|Booliano|Se definido como true, os membros podem adicionar e atualizar canais privados.|
|allowDeleteChannels|Booliano|Se definido como true, os membros podem excluir canais.|
|allowAddRemoveApps|Booliano|Se definido como true, os membros podem adicionar e remover aplicativos.|
|allowCreateUpdateRemoveTabs|Booliano|Se definido como true, os membros podem adicionar, atualizar e remover guias. |
|allowCreateUpdateRemoveConnectors|Booliano|Se definido como true, os membros podem adicionar, atualizar e remover conectores.|

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
