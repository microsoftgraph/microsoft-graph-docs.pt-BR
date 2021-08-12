---
title: Tipo de recurso searchResponse
description: Descrição da pesquisaResponse
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e071126b95cf0f82143c22f4523adcad640cb7df66718858a722e9f120177edc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54246560"
---
# <a name="searchresponse-resource-type"></a>Tipo de recurso searchResponse

Namespace: microsoft.graph

Representa os resultados de uma consulta de pesquisa e os termos usados para a consulta. 

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|hitsContainers|[coleção searchHitsContainer](searchhitscontainer.md)|Uma coleção de resultados de pesquisa.|
|searchTerms|Coleção de cadeias de caracteres|Contém os termos de pesquisa enviados na consulta de pesquisa inicial.|

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
  "hitsContainers": [{"@odata.type": "microsoft.graph.searchHitsContainer"}],
  "searchTerms": ["String"]
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

