---
title: Tipo de recurso mediaContentRatingGermany
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3242ffabc3f0bdac7e013ad6ffec97f6dd49d2de
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359968"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="95762-103">Tipo de recurso mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="95762-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="95762-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="95762-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95762-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="95762-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="95762-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="95762-106">Properties</span></span>
|<span data-ttu-id="95762-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95762-107">Property</span></span>|<span data-ttu-id="95762-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="95762-108">Type</span></span>|<span data-ttu-id="95762-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="95762-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95762-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="95762-110">movieRating</span></span>|[<span data-ttu-id="95762-111">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="95762-111">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="95762-112">Classificação de filmes selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="95762-112">Movies rating selected for Germany.</span></span> <span data-ttu-id="95762-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="95762-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="95762-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="95762-114">tvRating</span></span>|[<span data-ttu-id="95762-115">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="95762-115">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="95762-116">Classificação de TV selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="95762-116">TV rating selected for Germany.</span></span> <span data-ttu-id="95762-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="95762-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95762-118">Relações</span><span class="sxs-lookup"><span data-stu-id="95762-118">Relationships</span></span>
<span data-ttu-id="95762-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="95762-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95762-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="95762-120">JSON Representation</span></span>
<span data-ttu-id="95762-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="95762-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```




