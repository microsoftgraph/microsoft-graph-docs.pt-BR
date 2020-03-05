---
title: tipo de recurso searchHit
description: FORNEÇA UMA DESCRIÇÃO AQUI
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 722641b42a403565afcf7baa9de42af2b36a9dec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520925"
---
# <a name="searchhit-resource-type"></a>tipo de recurso searchHit

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um único resultado dentro da lista de resultados de pesquisa.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

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