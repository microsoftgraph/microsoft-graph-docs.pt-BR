---
title: tipo de recurso searchHit
description: Descrição da entidade searchHit
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: bad671657e46068263d3386eb0bb04026cfaa28e
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377954"
---
# <a name="searchhit-resource-type"></a>tipo de recurso searchHit

Namespace: microsoft.graph

Representa um único resultado dentro da lista de resultados de pesquisa.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|hitId|Cadeia de Caracteres|O identificador interno do item.|
|classificação|Int32|A classificação ou a ordem do resultado.|
|contentSource|Cadeia de Caracteres|O nome da fonte de conteúdo da qual o **externalItem** faz parte.|
|summary|Cadeia de Caracteres|Um resumo do resultado, se um resumo estiver disponível.|
|recurso|[entity](entity.md)|A representação subjacente do Microsoft Graph do resultado da pesquisa.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchHit",
  "baseType": null
}-->

```json
{
  "hitId": "String",
  "rank": 1,
  "summary": "String",
  "contentSource": "String",
  "resource": { "@odata.type": "microsoft.graph.entity" }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchHit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

