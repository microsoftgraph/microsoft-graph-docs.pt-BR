---
author: JeremyKelley
description: O recurso SearchResult indica que um item é a resposta a uma consulta de pesquisa.
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8ee83da0ffdd5d2ed577ba1b7165c05f5a63b1e8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063942"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="f8e23-103">Tipo de recurso SearchResult</span><span class="sxs-lookup"><span data-stu-id="f8e23-103">SearchResult resource type</span></span>

<span data-ttu-id="f8e23-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f8e23-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8e23-105">O recurso **SearchResult** indica que um item é a resposta a uma consulta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="f8e23-105">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="json-representation"></a><span data-ttu-id="f8e23-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f8e23-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f8e23-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f8e23-107">Properties</span></span>

| <span data-ttu-id="f8e23-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8e23-108">Property</span></span>            | <span data-ttu-id="f8e23-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8e23-109">Type</span></span>   | <span data-ttu-id="f8e23-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8e23-110">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="f8e23-111">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="f8e23-111">onClickTelemetryUrl</span></span> | <span data-ttu-id="f8e23-112">String</span><span class="sxs-lookup"><span data-stu-id="f8e23-112">String</span></span> | <span data-ttu-id="f8e23-p101">Uma URL de retorno de chamada que pode ser usada para registrar informações de telemetria. O aplicativo deve emitir um GET nesta URL se o usuário interagir com este item para melhorar a qualidade dos resultados.</span><span class="sxs-lookup"><span data-stu-id="f8e23-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="f8e23-115">Comentários</span><span class="sxs-lookup"><span data-stu-id="f8e23-115">Remarks</span></span>

<span data-ttu-id="f8e23-116">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="f8e23-116">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

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


