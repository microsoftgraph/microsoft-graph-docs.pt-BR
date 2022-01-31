---
title: Tipo de recurso searchResponse
description: 'Representa os resultados de uma consulta de pesquisa e os termos usados para a consulta. '
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 956bb2b38aefdf33f3c1b7096a2e599253e7e3af
ms.sourcegitcommit: a60e5e81cfa04b666a1df1111a1d91f6c11989e9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2022
ms.locfileid: "62282146"
---
# <a name="searchresponse-resource-type"></a>Tipo de recurso searchResponse

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa os resultados de uma consulta de pesquisa e os termos usados para a consulta. 

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|hitsContainers|[coleção searchHitsContainer](searchhitscontainer.md)|Uma coleção de resultados de pesquisa.|
|searchTerms|String collection|Contém os termos de pesquisa enviados na consulta de pesquisa inicial.|
|resultTemplates|[coleção resultTemplate](resultTemplate.md)|Um dicionário de resultTemplateIds e valores associados, que incluem o nome e o esquema JSON dos modelos de resultado.
|queryAlterationResponse|[alterationResponse](alterationResponse.md)|Fornece detalhes da resposta de alteração de consulta para correção ortográfica.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchResponse",
  "baseType": null
}-->

```json
{
  "queryAlterationResponse": {"@odata.type": "microsoft.graph.alterationResponse"},
  "hitsContainers": [{"@odata.type": "microsoft.graph.searchHitsContainer"}],
  "searchTerms": ["String"],
  "resultTemplates": [{"@odata.type":"microsoft.graph.resultTemplateDictionary"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

