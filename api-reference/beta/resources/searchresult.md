---
author: JeremyKelley
description: O recurso SearchResult indica que um item é a resposta a uma consulta de pesquisa.
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: cc819d8b81138ef279735d1daead9839d7f3b93f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520882"
---
# <a name="searchresult-resource-type"></a>Tipo de recurso SearchResult

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **SearchResult** indica que um item é a resposta a uma consulta de pesquisa.

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

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

<!--
{
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult",
  "suppressions": []
}
-->
