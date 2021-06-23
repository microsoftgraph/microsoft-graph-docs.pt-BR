---
title: Tipo de recurso conditionalAccessDevices
description: Representa dispositivos no escopo da política.
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: cbb542420228a4a383dea4e165323fbb6e8abb17
ms.sourcegitcommit: 9ac6bbab3df22e7629cf2bde796b527337c680aa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2021
ms.locfileid: "53082353"
---
# <a name="conditionalaccessdevices-resource-type"></a>Tipo de recurso conditionalAccessDevices

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa dispositivos no escopo da política.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| includeDevices | Conjunto de cadeias de caracteres | Estados no escopo da política. `All` é o único valor permitido. Não será possível definir *se deviceFIlter* estiver definido. |
| excludeDevices | Conjunto de cadeias de caracteres | Estados excluídos do escopo da política. Valores possíveis: `Compliant` , `DomainJoined` . Não será possível definir **se deviceFIlter** estiver definido. |
| deviceFilter | [conditionalAccessFilter](conditionalaccessfilter.md) | Filtrar definindo a regra de sintaxe de dispositivo dinâmico para incluir/excluir dispositivos. Um filtro pode usar propriedades de dispositivo (como atributos de extensão) para incluí-las/excluir. Não será possível definir **se includeDevices** ou **excludeDevices** estiver definido. |
| includeDeviceStates (preterido)| Conjunto de cadeias de caracteres | Estados no escopo da política. `All` é o único valor permitido. |
| excludeDeviceStates (preterido)| Conjunto de cadeias de caracteres | Estados excluídos do escopo da política. Valores possíveis: `Compliant` , `DomainJoined` . |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "includeDevices",
    "excludeDevices",
    "deviceFilter"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessDevices",
  "baseType": null
}-->

```json
{
  "includeDevices": [ "String" ],
  "excludeDevices": [ "String" ],
  "deviceFilter": {"@odata.type": "microsoft.graph.conditionalAccessFilter"}
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


