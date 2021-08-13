---
title: Tipo de recurso searchHit
description: Descrição da entidade searchHit
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3cc9d069e91dd8c8d51ba6b010c2c3ccc9dad01ac01695d6782e99bffea973e3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54138326"
---
# <a name="searchhit-resource-type"></a>Tipo de recurso searchHit

Namespace: microsoft.graph

Representa um único resultado na lista de resultados da pesquisa.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|hitId|Cadeia de caracteres|O identificador interno do item.|
|classificação|Int32|A classificação ou a ordem do resultado.|
|contentSource|String|O nome da fonte de conteúdo da **qual o externalItem** faz parte .|
|summary|Cadeia de caracteres|Um resumo do resultado, se um resumo estiver disponível.|
|recurso|[entity](entity.md)|A representação básica da Microsoft Graph do resultado da pesquisa.|

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

