---
title: Tipo de recurso conditionalAccessDevices
description: Representa dispositivos no escopo da política.
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a42e6023ace493c5efb230ffd53eb9c4caee7d16
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440525"
---
# <a name="conditionalaccessdevices-resource-type"></a>Tipo de recurso conditionalAccessDevices

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa dispositivos no escopo da política.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| includeDevices | Coleção de cadeias de caracteres | Estados no escopo da política. `All` é o único valor permitido. |
| excludeDevices | Coleção de cadeias de caracteres | Estados excluídos do escopo da política. Valores possíveis: `Compliant` , `DomainJoined` . |
| includeDeviceStates (preterido)| Coleção de cadeias de caracteres | Estados no escopo da política. `All` é o único valor permitido. |
| excludeDeviceStates (preterido)| Coleção de cadeias de caracteres | Estados excluídos do escopo da política. Valores possíveis: `Compliant` , `DomainJoined` . |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeDevices",
    "excludeDevices"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessDevices",
  "baseType": null
}-->

```json
{
  "includeDevices": [ "String" ],
  "excludeDevices": [ "String" ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessDevices resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


