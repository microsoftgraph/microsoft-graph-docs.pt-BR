---
title: Tipo de recurso searchHit
description: Descrição da entidade searchHit
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7c546483eea81e7d89a3a87ba5b8c0eb0ff48783
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53210329"
---
# <a name="searchhit-resource-type"></a>Tipo de recurso searchHit

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [search-api-deprecation](../../includes/search-api-deprecation.md)]

Representa um único resultado na lista de resultados da pesquisa.

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|hitId|String|O identificador interno do item.|
|classificação|Int32|A classificação ou a ordem do resultado.|
|contentSource|String|O nome da fonte de conteúdo da **qual o externalItem** faz parte .|
|summary|String|Um resumo do resultado, se um resumo estiver disponível.|
|resultTemplateId|String|ID do modelo de resultado para renderizar o resultado da pesquisa. Essa ID deve mapear para um layout de exibição no dicionário **resultTemplates,** incluído também na [pesquisaresponse.](searchresponse.md)|
|recurso|[entity](entity.md)|A representação básica da Microsoft Graph do resultado da pesquisa.|
|_id (preterido)|String| Renomeado como **hitId**. O identificador interno do item.|
|_score (preterido)|Int32|Renomeado como **classificação**. A pontuação ou a ordem do resultado.|
|_summary (preterido)|String|Renomeado como **resumo**. Um resumo do resultado (se o resumo estiver disponível).|
|_sortField (preterido)|String|Essa propriedade foi removida.|
|_source (preterido)|[entity](entity.md)|Renomeado como **recurso**. A representação Graph base do resultado da pesquisa.|

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
  "resultTemplateId": "String",
  "contentSource": "String",
  "resource": { "@odata.type": "microsoft.graph.entity" },
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

