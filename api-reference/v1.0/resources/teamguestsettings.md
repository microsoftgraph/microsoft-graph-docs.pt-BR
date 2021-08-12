---
title: Tipo de recurso teamGuestSettings
description: Configurações que definem se os convidados podem criar, atualizar ou excluir canais na equipe.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8b8c0a47135af606d2bfb83d190bd88d6af4ad65356c99096563f76053f9a9ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146353"
---
# <a name="teamguestsettings-resource-type"></a>Tipo de recurso teamGuestSettings

Namespace: microsoft.graph



Configurações configurar se os convidados podem criar, atualizar ou excluir canais na [equipe](team.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|Booliano|Se definido como true, os convidados podem adicionar e atualizar canais.|
|allowDeleteChannels|Booliano|Se definido como true, os convidados poderão excluir canais.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamGuestSettings"
}-->

```json
{
  "allowCreateUpdateChannels": true,
  "allowDeleteChannels": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's guestSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

