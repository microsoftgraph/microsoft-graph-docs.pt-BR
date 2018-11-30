---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SearchResult
ms.openlocfilehash: 7e6bd6e6ff48ae34e197955d16a3df1d539a3c05
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038463"
---
# <a name="searchresult-resource-type"></a><span data-ttu-id="d8a28-102">Tipo de recurso SearchResult</span><span class="sxs-lookup"><span data-stu-id="d8a28-102">SearchResult resource type</span></span>

> <span data-ttu-id="d8a28-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="d8a28-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d8a28-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d8a28-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d8a28-105">O recurso **SearchResult** indica que um item é a resposta a uma consulta de pesquisa.</span><span class="sxs-lookup"><span data-stu-id="d8a28-105">The **SearchResult** resource indicates than an item is the response to a search query.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8a28-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8a28-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="d8a28-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8a28-107">Properties</span></span>

| <span data-ttu-id="d8a28-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8a28-108">Property</span></span>            | <span data-ttu-id="d8a28-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8a28-109">Type</span></span>   | <span data-ttu-id="d8a28-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8a28-110">Description</span></span>
|:--------------------|:-------|:----------------------------------------------
| <span data-ttu-id="d8a28-111">onClickTelemetryUrl</span><span class="sxs-lookup"><span data-stu-id="d8a28-111">onClickTelemetryUrl</span></span> | <span data-ttu-id="d8a28-112">String</span><span class="sxs-lookup"><span data-stu-id="d8a28-112">String</span></span> | <span data-ttu-id="d8a28-p102">Uma URL de retorno de chamada que pode ser usada para registrar informações de telemetria. O aplicativo deve emitir um GET nesta URL se o usuário interagir com este item para melhorar a qualidade dos resultados.</span><span class="sxs-lookup"><span data-stu-id="d8a28-p102">A callback URL that can be used to record telemetry information. The application should issue a GET on this URL if the user interacts with this item to improve the quality of results.</span></span>

## <a name="remarks"></a><span data-ttu-id="d8a28-115">Comentários</span><span class="sxs-lookup"><span data-stu-id="d8a28-115">Remarks</span></span> 

<span data-ttu-id="d8a28-116">Para saber mais sobre as facetas de um DriveItem, confira [DriveItem](driveitem.md).</span><span class="sxs-lookup"><span data-stu-id="d8a28-116">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The search result facet indicates an item is from a search.",
  "keywords": "search result facet",
  "section": "documentation",
  "tocPath": "Facets/SearchResult"
} -->
