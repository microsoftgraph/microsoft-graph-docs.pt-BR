---
title: Tipo de recurso mediaContentRatingUnitedKingdom
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6f4810e8fa69e391b48c1048595a8da3c9766f4c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707147"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="7ac75-103">Tipo de recurso mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="7ac75-103">mediaContentRatingUnitedKingdom resource type</span></span>

<span data-ttu-id="7ac75-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ac75-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7ac75-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7ac75-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ac75-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7ac75-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ac75-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7ac75-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="7ac75-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ac75-108">Properties</span></span>
|<span data-ttu-id="7ac75-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ac75-109">Property</span></span>|<span data-ttu-id="7ac75-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ac75-110">Type</span></span>|<span data-ttu-id="7ac75-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ac75-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ac75-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="7ac75-112">movieRating</span></span>|[<span data-ttu-id="7ac75-113">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="7ac75-113">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="7ac75-114">Classificação de filmes selecionada para o Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="7ac75-114">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="7ac75-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="7ac75-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="7ac75-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="7ac75-116">tvRating</span></span>|[<span data-ttu-id="7ac75-117">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="7ac75-117">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="7ac75-118">Classificação de TV selecionada para o Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="7ac75-118">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="7ac75-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="7ac75-119">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ac75-120">Relações</span><span class="sxs-lookup"><span data-stu-id="7ac75-120">Relationships</span></span>
<span data-ttu-id="7ac75-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7ac75-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ac75-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ac75-122">JSON Representation</span></span>
<span data-ttu-id="7ac75-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7ac75-123">Here is a JSON representation of the resource.</span></span>
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





