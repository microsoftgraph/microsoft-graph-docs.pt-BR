---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SearchResult
localization_priority: Normal
ms.openlocfilehash: 025d18a48105ddb5834040aba5944a9bd408cfbc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562962"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="34efb-102">Tipo de recurso SearchResult</span><span class="sxs-lookup"><span data-stu-id="34efb-102">SearchResult resource type</span></span>

<span data-ttu-id="34efb-103">O recurso **SearchResult** indica que um item é a resposta a uma consulta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="34efb-103">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="34efb-104">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="34efb-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="34efb-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34efb-105">Properties</span></span>

| <span data-ttu-id="34efb-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34efb-106">Property</span></span>            | <span data-ttu-id="34efb-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="34efb-107">Type</span></span>   | <span data-ttu-id="34efb-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="34efb-108">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="34efb-109">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="34efb-109">onClickTelemetryUrl</span></span> | <span data-ttu-id="34efb-110">String</span><span class="sxs-lookup"><span data-stu-id="34efb-110">String</span></span> | <span data-ttu-id="34efb-p101">Uma URL de retorno de chamada que pode ser usada para registrar informações de telemetria. O aplicativo deve emitir um GET nesta URL se o usuário interagir com este item para melhorar a qualidade dos resultados.</span><span class="sxs-lookup"><span data-stu-id="34efb-p101">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="34efb-113">Comentários</span><span class="sxs-lookup"><span data-stu-id="34efb-113">Remarks</span></span> 

<span data-ttu-id="34efb-114">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="34efb-114">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->
