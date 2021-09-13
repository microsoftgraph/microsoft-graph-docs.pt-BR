---
title: Tipo de recurso searchHit
description: Descrição da entidade searchHit
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e64d4d3a2d7599df3ce6674abab352ab474ae18f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59137543"
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
|summary|String|Um resumo do resultado, se um resumo estiver disponível.|
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

