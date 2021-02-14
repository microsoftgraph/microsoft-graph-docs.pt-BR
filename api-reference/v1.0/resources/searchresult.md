---
author: JeremyKelley
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
description: O recurso SearchResult indica que um item é a resposta a uma consulta de pesquisa.
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: aac8ee9c4dea8ba7744e5c86d865b4d2f75a37d8
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240098"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="19acf-103">Tipo de recurso SearchResult</span><span class="sxs-lookup"><span data-stu-id="19acf-103">SearchResult resource type</span></span>

<span data-ttu-id="19acf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="19acf-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="19acf-105">O recurso **SearchResult** indica que um item é a resposta a uma consulta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="19acf-105">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="19acf-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="19acf-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="19acf-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="19acf-107">Properties</span></span>

| <span data-ttu-id="19acf-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="19acf-108">Property</span></span>            | <span data-ttu-id="19acf-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="19acf-109">Type</span></span>   | <span data-ttu-id="19acf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="19acf-110">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="19acf-111">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="19acf-111">onClickTelemetryUrl</span></span> | <span data-ttu-id="19acf-112">String</span><span class="sxs-lookup"><span data-stu-id="19acf-112">String</span></span> | <span data-ttu-id="19acf-p101">Uma URL de retorno de chamada que pode ser usada para registrar informações de telemetria. O aplicativo deve emitir um GET nesta URL se o usuário interagir com este item para melhorar a qualidade dos resultados.</span><span class="sxs-lookup"><span data-stu-id="19acf-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="19acf-115">Comentários</span><span class="sxs-lookup"><span data-stu-id="19acf-115">Remarks</span></span> 

<span data-ttu-id="19acf-116">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="19acf-116">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->

