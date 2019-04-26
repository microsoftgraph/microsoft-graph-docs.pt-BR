---
title: Tipo de recurso mediaContentRatingUnitedKingdom
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2c91558168922c4b608d62add941b69a5749bc9f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554461"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="357d5-103">Tipo de recurso mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="357d5-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="357d5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="357d5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="357d5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="357d5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="357d5-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="357d5-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="357d5-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="357d5-107">Properties</span></span>
|<span data-ttu-id="357d5-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="357d5-108">Property</span></span>|<span data-ttu-id="357d5-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="357d5-109">Type</span></span>|<span data-ttu-id="357d5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="357d5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="357d5-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="357d5-111">movieRating</span></span>|[<span data-ttu-id="357d5-112">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="357d5-112">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="357d5-113">Classificação de filmes selecionada para o Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="357d5-113">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="357d5-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="357d5-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="357d5-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="357d5-115">tvRating</span></span>|[<span data-ttu-id="357d5-116">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="357d5-116">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="357d5-117">Classificação de TV selecionada para o Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="357d5-117">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="357d5-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="357d5-118">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="357d5-119">Relações</span><span class="sxs-lookup"><span data-stu-id="357d5-119">Relationships</span></span>
<span data-ttu-id="357d5-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="357d5-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="357d5-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="357d5-121">JSON Representation</span></span>
<span data-ttu-id="357d5-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="357d5-122">Here is a JSON representation of the resource.</span></span>
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





