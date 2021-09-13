---
title: Tipo de recurso teamGuestSettings
description: Configurações que definem se os convidados podem criar, atualizar ou excluir canais na equipe.
ms.localizationpriority: medium
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 769930b28366b9918a92b9839331a421db5ff79a
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134336"
---
# <a name="teamguestsettings-resource-type"></a>Tipo de recurso teamGuestSettings

Namespace: microsoft.graph



Configurações configurar se os convidados podem criar, atualizar ou excluir canais na [equipe](team.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|Boolean|Se definido como true, os convidados podem adicionar e atualizar canais.|
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

