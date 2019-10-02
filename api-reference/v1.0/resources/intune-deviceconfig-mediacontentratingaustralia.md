---
title: Tipo de recurso mediaContentRatingAustralia
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 29e7c1d6668671afee5e382f6ba71e7d8f146df0
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360031"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="0ae4b-103">Tipo de recurso mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="0ae4b-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="0ae4b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0ae4b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ae4b-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0ae4b-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="0ae4b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0ae4b-106">Properties</span></span>
|<span data-ttu-id="0ae4b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ae4b-107">Property</span></span>|<span data-ttu-id="0ae4b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ae4b-108">Type</span></span>|<span data-ttu-id="0ae4b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ae4b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ae4b-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="0ae4b-110">movieRating</span></span>|[<span data-ttu-id="0ae4b-111">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="0ae4b-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="0ae4b-112">Classificação de filmes selecionada para a Austrália.</span><span class="sxs-lookup"><span data-stu-id="0ae4b-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="0ae4b-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="0ae4b-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="0ae4b-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="0ae4b-114">tvRating</span></span>|[<span data-ttu-id="0ae4b-115">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="0ae4b-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="0ae4b-116">Classificação de TV selecionada para a Austrália.</span><span class="sxs-lookup"><span data-stu-id="0ae4b-116">TV rating selected for Australia.</span></span> <span data-ttu-id="0ae4b-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="0ae4b-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ae4b-118">Relações</span><span class="sxs-lookup"><span data-stu-id="0ae4b-118">Relationships</span></span>
<span data-ttu-id="0ae4b-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0ae4b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ae4b-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0ae4b-120">JSON Representation</span></span>
<span data-ttu-id="0ae4b-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0ae4b-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```




