---
title: Tipo de recurso conditionalAccessDevices
description: Representa dispositivos no escopo da política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 94115e97c597bc34f03d843b8098f707ed39cd51
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761804"
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


