---
title: Tipo de recurso mediaContentRatingUnitedKingdom
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 947fd12d8219215b0828ef1c05d2d8b36f970f16
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252452"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="fec57-103">Tipo de recurso mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="fec57-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="fec57-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="fec57-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fec57-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="fec57-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="fec57-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fec57-106">Properties</span></span>
|<span data-ttu-id="fec57-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fec57-107">Property</span></span>|<span data-ttu-id="fec57-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="fec57-108">Type</span></span>|<span data-ttu-id="fec57-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="fec57-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fec57-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="fec57-110">movieRating</span></span>|[<span data-ttu-id="fec57-111">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="fec57-111">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="fec57-112">Classificação de filmes selecionada para o Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="fec57-112">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="fec57-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="fec57-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="fec57-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="fec57-114">tvRating</span></span>|[<span data-ttu-id="fec57-115">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="fec57-115">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="fec57-116">Classificação de TV selecionada para o Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="fec57-116">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="fec57-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="fec57-117">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fec57-118">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="fec57-118">Relationships</span></span>
<span data-ttu-id="fec57-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fec57-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fec57-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fec57-120">JSON Representation</span></span>
<span data-ttu-id="fec57-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fec57-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```



