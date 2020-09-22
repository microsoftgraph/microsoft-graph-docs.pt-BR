---
title: tipo de recurso searchEntity
description: Um objeto de nível superior representando o ponto de extremidade da API de pesquisa da Microsoft.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: cb6d5bdd5288a3f6098f33d3432a0e4f0d7ac8bd
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193830"
---
# <a name="searchentity-resource-type"></a>tipo de recurso searchEntity

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um objeto de nível superior representando o ponto de extremidade da API de pesquisa da Microsoft. Ela não se comporta como qualquer outro recurso no Graph, mas serve como uma âncora para a ação de [consulta](../api/search-query.md) . 

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Methods
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[query](../api/search-query.md) |coleção [searchResponse](searchresponse.md) | Executa a consulta especificada no corpo da solicitação.  |

## <a name="properties"></a>Propriedades
Nenhum.

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.searchEntity",
  "baseType": "microsoft.graph.entity"
}
-->
``` json
{
  
}
```


## <a name="next-steps"></a>Próximas etapas

Explore a ação de [consulta](../api/search-query.md) .


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "A top level object representing the Microsoft Search API endpoint.",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


