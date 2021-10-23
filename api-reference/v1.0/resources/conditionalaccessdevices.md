---
title: Tipo de recurso conditionalAccessDevices
description: Representa dispositivos no escopo da política.
ms.localizationpriority: medium
author: sandeo
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 419a9b92626fb3c3693f5974119d677ef50d5b26
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561749"
---
# <a name="conditionalaccessdevices-resource-type"></a>Tipo de recurso conditionalAccessDevices

Namespace: microsoft.graph

Representa dispositivos no escopo da política.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
| deviceFilter | [conditionalAccessFilter](conditionalaccessfilter.md) | Filtro que define a regra de sintaxe de dispositivo dinâmico para incluir/excluir dispositivos. Um filtro pode usar propriedades de dispositivo (como atributos de extensão) para incluí-las/excluir. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "deviceFilter"
  ],
  "@odata.type": "microsoft.graph.conditionalAccessDevices",
  "baseType": null
}-->

```json
{
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


