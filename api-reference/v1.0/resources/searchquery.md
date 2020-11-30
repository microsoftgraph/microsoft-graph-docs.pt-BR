---
title: tipo de recurso searchQuery
description: searchQuery
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3745083b404a8de6f68844af9b1767ac2319059f
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377955"
---
# <a name="searchquery-resource-type"></a>tipo de recurso searchQuery

Namespace: microsoft.graph

Representa uma consulta de pesquisa que contém termos de pesquisa e filtros opcionais.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|queryString|Cadeia de Caracteres|A consulta de pesquisa que contém os termos da pesquisa. Obrigatório.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchQuery",
  "baseType": null
}-->

```json
{
  "queryString": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchQuery resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

