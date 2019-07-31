---
author: JeremyKelley
description: O recurso SearchResult indica que um item é a resposta a uma consulta de pesquisa.
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 716a8147c9041ceee64993f9e90ad2f0f9ecb9e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008604"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="4687f-103">Tipo de recurso SearchResult</span><span class="sxs-lookup"><span data-stu-id="4687f-103">SearchResult resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4687f-104">O recurso **SearchResult** indica que um item é a resposta a uma consulta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="4687f-104">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4687f-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4687f-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="4687f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4687f-106">Properties</span></span>

| <span data-ttu-id="4687f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4687f-107">Property</span></span>            | <span data-ttu-id="4687f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="4687f-108">Type</span></span>   | <span data-ttu-id="4687f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4687f-109">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="4687f-110">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="4687f-110">onClickTelemetryUrl</span></span> | <span data-ttu-id="4687f-111">String</span><span class="sxs-lookup"><span data-stu-id="4687f-111">String</span></span> | <span data-ttu-id="4687f-p101">Uma URL de retorno de chamada que pode ser usada para registrar informações de telemetria. O aplicativo deve emitir um GET nesta URL se o usuário interagir com este item para melhorar a qualidade dos resultados.</span><span class="sxs-lookup"><span data-stu-id="4687f-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="4687f-114">Comentários</span><span class="sxs-lookup"><span data-stu-id="4687f-114">Remarks</span></span> 

<span data-ttu-id="4687f-115">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="4687f-115">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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
