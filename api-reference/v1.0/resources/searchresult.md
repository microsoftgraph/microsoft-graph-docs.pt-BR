---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
description: O recurso SearchResult indica que um item é a resposta a uma consulta de pesquisa.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 571e063f8125fb587cbcfff07b4414b5c948d829
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984128"
---
# <a name="searchresult-resource-type"></a>Tipo de recurso SearchResult

Namespace: microsoft.graph

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

