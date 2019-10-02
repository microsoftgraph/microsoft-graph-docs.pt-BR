---
title: Tipo de recurso mediaContentRatingNewZealand
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b6b90142c50237706ac7e9c887d3a848224c1ec9
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356664"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="55b02-103">Tipo de recurso mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="55b02-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="55b02-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="55b02-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55b02-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="55b02-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="55b02-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="55b02-106">Properties</span></span>
|<span data-ttu-id="55b02-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55b02-107">Property</span></span>|<span data-ttu-id="55b02-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="55b02-108">Type</span></span>|<span data-ttu-id="55b02-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="55b02-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55b02-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="55b02-110">movieRating</span></span>|[<span data-ttu-id="55b02-111">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="55b02-111">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="55b02-112">Classificação de filmes selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="55b02-112">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="55b02-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="55b02-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="55b02-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="55b02-114">tvRating</span></span>|[<span data-ttu-id="55b02-115">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="55b02-115">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="55b02-116">Classificação de TV selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="55b02-116">TV rating selected for New Zealand.</span></span> <span data-ttu-id="55b02-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="55b02-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55b02-118">Relações</span><span class="sxs-lookup"><span data-stu-id="55b02-118">Relationships</span></span>
<span data-ttu-id="55b02-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="55b02-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="55b02-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="55b02-120">JSON Representation</span></span>
<span data-ttu-id="55b02-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="55b02-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```




