---
title: Tipo de recurso mediaContentRatingUnitedKingdom
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0169e26be7590031ba5e7e7f676d51f69a526452
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160176"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="53f06-103">Tipo de recurso mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="53f06-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="53f06-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="53f06-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53f06-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="53f06-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53f06-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="53f06-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="53f06-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="53f06-107">Properties</span></span>
|<span data-ttu-id="53f06-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53f06-108">Property</span></span>|<span data-ttu-id="53f06-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="53f06-109">Type</span></span>|<span data-ttu-id="53f06-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="53f06-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53f06-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="53f06-111">movieRating</span></span>|[<span data-ttu-id="53f06-112">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="53f06-112">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="53f06-113">Classificação de filmes selecionada para o Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="53f06-113">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="53f06-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="53f06-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="53f06-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="53f06-115">tvRating</span></span>|[<span data-ttu-id="53f06-116">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="53f06-116">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="53f06-117">Classificação de TV selecionada para o Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="53f06-117">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="53f06-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="53f06-118">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53f06-119">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="53f06-119">Relationships</span></span>
<span data-ttu-id="53f06-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="53f06-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="53f06-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="53f06-121">JSON Representation</span></span>
<span data-ttu-id="53f06-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="53f06-122">Here is a JSON representation of the resource.</span></span>
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




