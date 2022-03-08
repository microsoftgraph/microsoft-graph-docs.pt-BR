---
title: Tipo de recurso searchEntity
description: Um objeto de nível superior que representa o ponto de extremidade Pesquisa da Microsoft API.
ms.localizationpriority: medium
author: nmoreau
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 39f5213e9be29f9fd87332513c3d0b090e3d3e1f
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335182"
---
# <a name="searchentity-resource-type"></a>Tipo de recurso searchEntity

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um objeto de nível superior que representa o ponto de extremidade Pesquisa da Microsoft API.

Ele serve como âncora para a ação [de](../api/search-query.md) consulta e relações de resposta de pesquisa, como acrônimos, [indicadores](../resources/search-bookmark.md) e [qnas](../resources/search-qna.md).[](../resources/search-acronym.md) 

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[query](../api/search-query.md) |[Coleção searchResponse](searchresponse.md) | Execute uma consulta de pesquisa especificada.   |

## <a name="properties"></a>Propriedades
Nenhum.

## <a name="relationships"></a>Relações
| Relação | Tipo |Descrição|
|:---------------|:--------|:----------|
| acrônimos | [coleção microsoft.graph.search.acronym](../resources/search-acronym.md) | Resposta administrativa em Pesquisa da Microsoft para definir acrônimos comuns em uma organização.  |
| indicadores | [coleção microsoft.graph.search.bookmark](../resources/search-bookmark.md) | Resposta administrativa em Pesquisa da Microsoft resultados para consultas de pesquisa comuns em uma organização. |
| qnas | [coleção microsoft.graph.search.qna](../resources/search-qna.md) | Resposta administrativa em Pesquisa da Microsoft resultados que fornecem respostas para palavras-chave de pesquisa específicas em uma organização. |


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


## <a name="see-also"></a>Confira também

[query](../api/search-query.md)


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "A top level object representing the Microsoft Search API endpoint.",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


