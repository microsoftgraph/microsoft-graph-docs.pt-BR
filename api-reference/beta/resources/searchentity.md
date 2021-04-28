---
title: Tipo de recurso searchEntity
description: Um objeto de nível superior que representa o ponto de extremidade da API de Pesquisa da Microsoft.
localization_priority: Normal
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: d62292b3a4890589d72214a3544059eaf8af8817
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067128"
---
# <a name="searchentity-resource-type"></a>Tipo de recurso searchEntity

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um objeto de nível superior que representa o ponto de extremidade da API de Pesquisa da Microsoft. Ele não se comporta como qualquer outro recurso no Graph, mas serve como uma âncora para a [ação de](../api/search-query.md) consulta. 

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[query](../api/search-query.md) |[searchResponse](searchresponse.md) | Executa a consulta especificada no corpo da solicitação.  |

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

Explore [a ação de](../api/search-query.md) consulta.


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "A top level object representing the Microsoft Search API endpoint.",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


