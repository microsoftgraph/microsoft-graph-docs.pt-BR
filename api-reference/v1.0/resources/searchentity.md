---
title: tipo de recurso searchEntity
description: Um objeto de nível superior representando o ponto de extremidade da API de pesquisa da Microsoft.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 4382deb0b23d051eb7b713661c3a61035e5ceafa
ms.sourcegitcommit: 5345c2f3265ede107fa0faaff7a3f1c2afee3810
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377958"
---
# <a name="searchentity-resource-type"></a>tipo de recurso searchEntity

Namespace: microsoft.graph

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


