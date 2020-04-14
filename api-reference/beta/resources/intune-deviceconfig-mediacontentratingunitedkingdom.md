---
title: Tipo de recurso mediaContentRatingUnitedKingdom
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 794e0cb0a461a9ff23c7c3351925dd3efd7ebf89
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437144"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="41e20-103">Tipo de recurso mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="41e20-103">mediaContentRatingUnitedKingdom resource type</span></span>

<span data-ttu-id="41e20-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41e20-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41e20-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="41e20-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41e20-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="41e20-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41e20-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="41e20-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="41e20-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="41e20-108">Properties</span></span>
|<span data-ttu-id="41e20-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="41e20-109">Property</span></span>|<span data-ttu-id="41e20-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="41e20-110">Type</span></span>|<span data-ttu-id="41e20-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="41e20-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41e20-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="41e20-112">movieRating</span></span>|[<span data-ttu-id="41e20-113">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="41e20-113">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="41e20-114">Classificação de filmes selecionada para o Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="41e20-114">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="41e20-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="41e20-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="41e20-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="41e20-116">tvRating</span></span>|[<span data-ttu-id="41e20-117">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="41e20-117">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="41e20-118">Classificação de TV selecionada para o Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="41e20-118">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="41e20-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="41e20-119">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="41e20-120">Relações</span><span class="sxs-lookup"><span data-stu-id="41e20-120">Relationships</span></span>
<span data-ttu-id="41e20-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="41e20-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="41e20-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="41e20-122">JSON Representation</span></span>
<span data-ttu-id="41e20-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="41e20-123">Here is a JSON representation of the resource.</span></span>
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



