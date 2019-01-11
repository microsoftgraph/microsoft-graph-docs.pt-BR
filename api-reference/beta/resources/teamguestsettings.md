---
title: tipo de recurso de teamGuestSettings
description: Configurações para configurar se os convidados podem criar, atualizar ou excluir canais na equipe de.
localization_priority: Normal
ms.openlocfilehash: 15644f3761329589a4d770e777ae5fd63751e6be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851538"
---
# <a name="teamguestsettings-resource-type"></a>tipo de recurso de teamGuestSettings

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Configurações para configurar se os convidados podem criar, atualizar ou excluir canais em que a [equipe](team.md).

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|allowCreateUpdateChannels|Booliano|Se definido como true, convidados pode adicionar e atualizar os canais.|
|allowDeleteChannels|Booliano|Se definido como true, convidados pode excluir canais.|

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
