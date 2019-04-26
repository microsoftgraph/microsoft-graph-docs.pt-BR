---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
ms.openlocfilehash: 74743839d55dd5a8fc52661fac4a071d7a1730bc
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343476"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="36d30-102">Tipo de recurso SearchResult</span><span class="sxs-lookup"><span data-stu-id="36d30-102">SearchResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="36d30-103">O recurso **SearchResult** indica que um item é a resposta a uma consulta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="36d30-103">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="36d30-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="36d30-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="36d30-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="36d30-105">Properties</span></span>

| <span data-ttu-id="36d30-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="36d30-106">Property</span></span>            | <span data-ttu-id="36d30-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="36d30-107">Type</span></span>   | <span data-ttu-id="36d30-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="36d30-108">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="36d30-109">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="36d30-109">onClickTelemetryUrl</span></span> | <span data-ttu-id="36d30-110">String</span><span class="sxs-lookup"><span data-stu-id="36d30-110">String</span></span> | <span data-ttu-id="36d30-p101">Uma URL de retorno de chamada que pode ser usada para registrar informações de telemetria. O aplicativo deve emitir um GET nesta URL se o usuário interagir com este item para melhorar a qualidade dos resultados.</span><span class="sxs-lookup"><span data-stu-id="36d30-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="36d30-113">Comentários</span><span class="sxs-lookup"><span data-stu-id="36d30-113">Remarks</span></span> 

<span data-ttu-id="36d30-114">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="36d30-114">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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
