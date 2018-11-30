---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SearchResult
ms.openlocfilehash: 120f1805196e40d652bd2fcd409f4ee3cd3203fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004460"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="6e85a-102">Tipo de recurso SearchResult</span><span class="sxs-lookup"><span data-stu-id="6e85a-102">SearchResult resource type</span></span>

<span data-ttu-id="6e85a-103">O recurso **SearchResult** indica que um item é a resposta a uma consulta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="6e85a-103">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e85a-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e85a-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="6e85a-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e85a-105">Properties</span></span>

| <span data-ttu-id="6e85a-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e85a-106">Property</span></span>            | <span data-ttu-id="6e85a-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e85a-107">Type</span></span>   | <span data-ttu-id="6e85a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e85a-108">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="6e85a-109">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="6e85a-109">onClickTelemetryUrl</span></span> | <span data-ttu-id="6e85a-110">String</span><span class="sxs-lookup"><span data-stu-id="6e85a-110">String</span></span> | <span data-ttu-id="6e85a-p101">Uma URL de retorno de chamada que pode ser usada para registrar informações de telemetria. O aplicativo deve emitir um GET nesta URL se o usuário interagir com este item para melhorar a qualidade dos resultados.</span><span class="sxs-lookup"><span data-stu-id="6e85a-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="6e85a-113">Comentários</span><span class="sxs-lookup"><span data-stu-id="6e85a-113">Remarks</span></span> 

<span data-ttu-id="6e85a-114">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="6e85a-114">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->
