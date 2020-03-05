---
title: tipo de recurso conditionalAccessDeviceStates
description: Representa os Estados do dispositivo no escopo da política.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ff61b1d9713a0da322d01e3c302ebefc98dbee46
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507552"
---
# <a name="conditionalaccessdevicestates-resource-type"></a>tipo de recurso conditionalAccessDeviceStates

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os Estados do dispositivo no escopo da política.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| includeStates | String collection | Estados no escopo da política. `All`é o único valor permitido. |
| excludeStates | String collection | Estados excluídos do escopo da política. Valores possíveis: `Compliant`, `DomainJoined`. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeStates",
    "excludeStates"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessDeviceStates",
  "baseType": null
}-->

```json
{
  "includeStates": [ "String" ],
  "excludeStates": [ "String" ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessDeviceStates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->