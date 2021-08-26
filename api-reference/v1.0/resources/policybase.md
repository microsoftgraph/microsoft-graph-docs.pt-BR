---
title: Tipo de recurso policyBase
description: Representa um tipo de base abstrato para tipos de política herdado.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2918543536f62627f7c2a742009c3d67012353b4
ms.sourcegitcommit: 998c63e6290cfb5ad4a6bd3eb3e249d282f962a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/26/2021
ms.locfileid: "58531219"
---
# <a name="policybase-resource-type"></a>Tipo de recurso policyBase

Namespace: microsoft.graph

Representa um tipo de base abstrato para tipos de política herdado. Herda de [directoryObject](directoryobject.md).

## <a name="methods"></a>Métodos

Nenhum

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres| Identificador exclusivo dessa política. Somente leitura. Herdado de [directoryObject](directoryobject.md).|
|descrição|Cadeia de caracteres| Descrição dessa política.|
|displayName|Cadeia de caracteres| Nome de exibição para esta política. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.policyBase",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "policyBase resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
