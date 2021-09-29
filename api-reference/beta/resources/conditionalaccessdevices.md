---
title: Tipo de recurso conditionalAccessDevices
description: Representa dispositivos no escopo da política.
ms.localizationpriority: medium
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 0c4bc7721566bd8210830e51dbe820b1b44813e1
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996364"
---
# <a name="conditionalaccessdevices-resource-type"></a>Tipo de recurso conditionalAccessDevices

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa dispositivos no escopo da política.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| includeDevices | Coleção de cadeia de caracteres | Estados no escopo da política. `All` é o único valor permitido. Não será possível definir *se deviceFIlter* estiver definido. |
| excludeDevices | Coleção de cadeia de caracteres | Estados excluídos do escopo da política. Valores possíveis: `Compliant` , `DomainJoined` . Não será possível definir **se deviceFIlter** estiver definido. |
| deviceFilter | [conditionalAccessFilter](conditionalaccessfilter.md) | Filtro que define a regra de sintaxe de dispositivo dinâmico para incluir/excluir dispositivos. Um filtro pode usar propriedades de dispositivo (como atributos de extensão) para incluí-las/excluir. Não será possível definir **se includeDevices** ou **excludeDevices** estiver definido. |
| includeDeviceStates (preterido)| Coleção de cadeia de caracteres | Estados no escopo da política. `All` é o único valor permitido. |
| excludeDeviceStates (preterido)| Coleção de cadeia de caracteres | Estados excluídos do escopo da política. Valores possíveis: `Compliant` , `DomainJoined` . |

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


