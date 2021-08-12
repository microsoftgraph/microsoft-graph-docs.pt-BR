---
author: JeremyKelley
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
description: O recurso SearchResult indica que um item é a resposta a uma consulta de pesquisa.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 5b07e58e7ac9e568e6f1edad75be254b02dbc405fe2520f171abbf0af90365b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180464"
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

