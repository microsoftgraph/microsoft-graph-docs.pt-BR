---
title: Tipo de recurso mediaContentRatingFrance
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 40f4650a99c9914257e868ac7d84f34ed1369276
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359996"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="767f5-103">Tipo de recurso mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="767f5-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="767f5-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="767f5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="767f5-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="767f5-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="767f5-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="767f5-106">Properties</span></span>
|<span data-ttu-id="767f5-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="767f5-107">Property</span></span>|<span data-ttu-id="767f5-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="767f5-108">Type</span></span>|<span data-ttu-id="767f5-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="767f5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="767f5-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="767f5-110">movieRating</span></span>|[<span data-ttu-id="767f5-111">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="767f5-111">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="767f5-112">Classificação de filmes selecionada para a França.</span><span class="sxs-lookup"><span data-stu-id="767f5-112">Movies rating selected for France.</span></span> <span data-ttu-id="767f5-113">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="767f5-113">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="767f5-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="767f5-114">tvRating</span></span>|[<span data-ttu-id="767f5-115">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="767f5-115">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="767f5-116">Classificação de TV selecionada para a França.</span><span class="sxs-lookup"><span data-stu-id="767f5-116">TV rating selected for France.</span></span> <span data-ttu-id="767f5-117">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="767f5-117">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="767f5-118">Relações</span><span class="sxs-lookup"><span data-stu-id="767f5-118">Relationships</span></span>
<span data-ttu-id="767f5-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="767f5-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="767f5-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="767f5-120">JSON Representation</span></span>
<span data-ttu-id="767f5-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="767f5-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```




