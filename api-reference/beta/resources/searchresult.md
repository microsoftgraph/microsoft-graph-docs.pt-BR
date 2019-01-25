---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
ms.openlocfilehash: c50f90787627732843e152a37a469c03340aa370
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511069"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="9022a-102">Tipo de recurso SearchResult</span><span class="sxs-lookup"><span data-stu-id="9022a-102">SearchResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9022a-103">O recurso **SearchResult** indica que um item é a resposta a uma consulta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="9022a-103">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9022a-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9022a-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="9022a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9022a-105">Properties</span></span>

| <span data-ttu-id="9022a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9022a-106">Property</span></span>            | <span data-ttu-id="9022a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="9022a-107">Type</span></span>   | <span data-ttu-id="9022a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9022a-108">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="9022a-109">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="9022a-109">onClickTelemetryUrl</span></span> | <span data-ttu-id="9022a-110">String</span><span class="sxs-lookup"><span data-stu-id="9022a-110">String</span></span> | <span data-ttu-id="9022a-p101">Uma URL de retorno de chamada que pode ser usada para registrar informações de telemetria. O aplicativo deve emitir um GET nesta URL se o usuário interagir com este item para melhorar a qualidade dos resultados.</span><span class="sxs-lookup"><span data-stu-id="9022a-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="9022a-113">Comentários</span><span class="sxs-lookup"><span data-stu-id="9022a-113">Remarks</span></span> 

<span data-ttu-id="9022a-114">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="9022a-114">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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
