---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
ms.openlocfilehash: ee6825860f5c1ed82c368b53eb3510175e7d3a11
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2019
ms.locfileid: "30481227"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="71946-102">Tipo de recurso SearchResult</span><span class="sxs-lookup"><span data-stu-id="71946-102">SearchResult resource type</span></span>

<span data-ttu-id="71946-103">O recurso **SearchResult** indica que um item é a resposta a uma consulta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="71946-103">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="71946-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="71946-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="71946-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="71946-105">Properties</span></span>

| <span data-ttu-id="71946-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="71946-106">Property</span></span>            | <span data-ttu-id="71946-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="71946-107">Type</span></span>   | <span data-ttu-id="71946-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="71946-108">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="71946-109">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="71946-109">onClickTelemetryUrl</span></span> | <span data-ttu-id="71946-110">String</span><span class="sxs-lookup"><span data-stu-id="71946-110">String</span></span> | <span data-ttu-id="71946-p101">Uma URL de retorno de chamada que pode ser usada para registrar informações de telemetria. O aplicativo deve emitir um GET nesta URL se o usuário interagir com este item para melhorar a qualidade dos resultados.</span><span class="sxs-lookup"><span data-stu-id="71946-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="71946-113">Comentários</span><span class="sxs-lookup"><span data-stu-id="71946-113">Remarks</span></span> 

<span data-ttu-id="71946-114">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="71946-114">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->
