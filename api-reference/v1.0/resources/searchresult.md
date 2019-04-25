---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
ms.openlocfilehash: ee6825860f5c1ed82c368b53eb3510175e7d3a11
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579195"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="f5a3f-102">Tipo de recurso SearchResult</span><span class="sxs-lookup"><span data-stu-id="f5a3f-102">SearchResult resource type</span></span>

<span data-ttu-id="f5a3f-103">O recurso **SearchResult** indica que um item é a resposta a uma consulta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="f5a3f-103">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5a3f-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f5a3f-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f5a3f-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f5a3f-105">Properties</span></span>

| <span data-ttu-id="f5a3f-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5a3f-106">Property</span></span>            | <span data-ttu-id="f5a3f-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5a3f-107">Type</span></span>   | <span data-ttu-id="f5a3f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5a3f-108">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="f5a3f-109">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="f5a3f-109">onClickTelemetryUrl</span></span> | <span data-ttu-id="f5a3f-110">String</span><span class="sxs-lookup"><span data-stu-id="f5a3f-110">String</span></span> | <span data-ttu-id="f5a3f-p101">Uma URL de retorno de chamada que pode ser usada para registrar informações de telemetria. O aplicativo deve emitir um GET nesta URL se o usuário interagir com este item para melhorar a qualidade dos resultados.</span><span class="sxs-lookup"><span data-stu-id="f5a3f-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="f5a3f-113">Comentários</span><span class="sxs-lookup"><span data-stu-id="f5a3f-113">Remarks</span></span> 

<span data-ttu-id="f5a3f-114">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="f5a3f-114">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->
