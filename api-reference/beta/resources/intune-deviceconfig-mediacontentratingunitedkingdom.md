---
title: Tipo de recurso mediaContentRatingUnitedKingdom
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5dc8a19664e0d1b9d80451af88686be59b179780
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993780"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="52914-103">Tipo de recurso mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="52914-103">mediaContentRatingUnitedKingdom resource type</span></span>

<span data-ttu-id="52914-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52914-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52914-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="52914-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52914-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="52914-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52914-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="52914-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="52914-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52914-108">Properties</span></span>
|<span data-ttu-id="52914-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52914-109">Property</span></span>|<span data-ttu-id="52914-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="52914-110">Type</span></span>|<span data-ttu-id="52914-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="52914-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52914-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="52914-112">movieRating</span></span>|[<span data-ttu-id="52914-113">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="52914-113">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="52914-114">Classificação de filmes selecionada para o Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="52914-114">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="52914-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="52914-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="52914-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="52914-116">tvRating</span></span>|[<span data-ttu-id="52914-117">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="52914-117">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="52914-118">Classificação de TV selecionada para o Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="52914-118">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="52914-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="52914-119">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52914-120">Relações</span><span class="sxs-lookup"><span data-stu-id="52914-120">Relationships</span></span>
<span data-ttu-id="52914-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="52914-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="52914-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52914-122">JSON Representation</span></span>
<span data-ttu-id="52914-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52914-123">Here is a JSON representation of the resource.</span></span>
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






