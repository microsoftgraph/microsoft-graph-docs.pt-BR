---
title: Tipo de recurso teamMemberSettings
description: Configurações para configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots na equipe.
ms.localizationpriority: medium
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 215efff423e417d83f2416021b877c8d0c08897e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59049491"
---
# <a name="teammembersettings-resource-type"></a>Tipo de recurso teamMemberSettings

Namespace: microsoft.graph



Configurações configurar se os membros podem executar determinadas ações, por exemplo, criar canais e adicionar bots, na [equipe](team.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowCreatePrivateChannels|Boolean|Se definido como true, os membros podem adicionar e atualizar canais privados.|
|allowCreateUpdateChannels|Boolean|Se definido como true, os membros podem adicionar e atualizar canais.|
|allowDeleteChannels|Booliano|Se definido como true, os membros poderão excluir canais.|
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
  "allowCreatePrivateChannels": true,
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true,
  "allowAddRemoveApps": true,
  "allowCreateUpdateRemoveTabs": true,
  "allowCreateUpdateRemoveConnectors": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's memberSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

