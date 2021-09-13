---
title: Tipo de recurso policyBase
description: Representa um tipo de base abstrato para tipos de política herdado.
ms.localizationpriority: medium
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 6795065e7edbf9d31936007e842c24882d138185
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59098479"
---
# <a name="policybase-resource-type"></a>Tipo de recurso policyBase

Namespace: microsoft.graph

Representa um tipo de base abstrato para tipos de política herdado. Herda de [directoryObject](directoryobject.md).

## <a name="methods"></a>Métodos

Nenhum(a)

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|id|Cadeia de caracteres| Identificador exclusivo dessa política. Somente leitura. Herdado de [directoryObject](directoryobject.md).|
|description|String| Descrição dessa política. Obrigatório.|
|displayName|Cadeia de caracteres| Nome de exibição para esta política. Obrigatório. |

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
