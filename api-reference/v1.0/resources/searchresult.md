---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SearchResult
ms.openlocfilehash: 33ce07c947d858f05844dd9dc2589379131c9dbb
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="searchresult-resource-type"></a>Tipo de recurso SearchResult

O recurso **SearchResult** indica que um item é a resposta a uma consulta de pesquisa.

## <a name="json-representation"></a>Representação JSON

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "onClickTelemtryUrl" ],
  "@odata.type": "microsoft.graph.searchResult"
}-->

```json
{
  "onClickTelemetryUrl": "url"
}
```

## <a name="properties"></a>Propriedades

| Propriedade            | Tipo   | Descrição
|:--------------------|:-------|:----------------------------------------------
| onClickTelemetryUrl | String | Uma URL de retorno de chamada que pode ser usada para registrar informações de telemetria. O aplicativo deve emitir um GET nesta URL se o usuário interagir com este item para melhorar a qualidade dos resultados.

## <a name="remarks"></a>Comentários 

Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->
