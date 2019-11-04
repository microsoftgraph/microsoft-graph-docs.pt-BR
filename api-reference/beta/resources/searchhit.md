---
title: tipo de recurso searchHit
description: FORNEÇA UMA DESCRIÇÃO AQUI
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 2ce5671933589f6066698df3e082390207474b49
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939863"
---
# <a name="searchhit-resource-type"></a>tipo de recurso searchHit

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um único resultado dentro da lista de resultados de pesquisa.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|_id|String|O identificador interno do item.|
|_score|Int32|A pontuação ou a ordem do resultado.|
|_sortField|String|A ordem de classificação usada. Pode ser DateTime ou relevância.|
|_summary|String|Um resumo do resultado (se o resumo estiver disponível).|
|_source|[entity](entity.md)|A representação de gráfico subjacente do resultado da pesquisa.|

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
  "_id": "String",
  "_score": 1024,
  "_sortField": "String",
  "_summary": "String",
  "_source": { "@odata.type": "microsoft.graph.entity" }
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