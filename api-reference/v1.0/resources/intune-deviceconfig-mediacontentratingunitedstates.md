---
title: Tipo de recurso mediaContentRatingUnitedStates
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ee961024a526300b1bbf7ebb186df69ce0337f78
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366584"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="65350-103">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="65350-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="65350-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="65350-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65350-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="65350-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="65350-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="65350-106">Properties</span></span>
|<span data-ttu-id="65350-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65350-107">Property</span></span>|<span data-ttu-id="65350-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="65350-108">Type</span></span>|<span data-ttu-id="65350-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="65350-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65350-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="65350-110">movieRating</span></span>|[<span data-ttu-id="65350-111">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="65350-111">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="65350-112">Classificação de filmes selecionada para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="65350-112">Movies rating selected for United States.</span></span> <span data-ttu-id="65350-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="65350-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="65350-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="65350-114">tvRating</span></span>|[<span data-ttu-id="65350-115">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="65350-115">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="65350-116">Classificação de TV selecionada para Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="65350-116">TV rating selected for United States.</span></span> <span data-ttu-id="65350-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="65350-117">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65350-118">Relações</span><span class="sxs-lookup"><span data-stu-id="65350-118">Relationships</span></span>
<span data-ttu-id="65350-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="65350-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65350-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="65350-120">JSON Representation</span></span>
<span data-ttu-id="65350-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="65350-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```




