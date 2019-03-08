---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
ms.openlocfilehash: 025d18a48105ddb5834040aba5944a9bd408cfbc
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480380"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="a0ee8-102">Tipo de recurso SearchResult</span><span class="sxs-lookup"><span data-stu-id="a0ee8-102">SearchResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0ee8-103">O recurso **SearchResult** indica que um item é a resposta a uma consulta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="a0ee8-103">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0ee8-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0ee8-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="a0ee8-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0ee8-105">Properties</span></span>

| <span data-ttu-id="a0ee8-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0ee8-106">Property</span></span>            | <span data-ttu-id="a0ee8-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0ee8-107">Type</span></span>   | <span data-ttu-id="a0ee8-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0ee8-108">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="a0ee8-109">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="a0ee8-109">onClickTelemetryUrl</span></span> | <span data-ttu-id="a0ee8-110">String</span><span class="sxs-lookup"><span data-stu-id="a0ee8-110">String</span></span> | <span data-ttu-id="a0ee8-p101">Uma URL de retorno de chamada que pode ser usada para registrar informações de telemetria. O aplicativo deve emitir um GET nesta URL se o usuário interagir com este item para melhorar a qualidade dos resultados.</span><span class="sxs-lookup"><span data-stu-id="a0ee8-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="a0ee8-113">Comentários</span><span class="sxs-lookup"><span data-stu-id="a0ee8-113">Remarks</span></span> 

<span data-ttu-id="a0ee8-114">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="a0ee8-114">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult",
  "suppressions": [
    "Error: /api-reference/beta/resources/searchresult.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
