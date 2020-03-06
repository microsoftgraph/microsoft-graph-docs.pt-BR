---
title: Tipo de recurso mediaContentRatingUnitedKingdom
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 37bf3226da7483f9185723d42ed3442cfc16117c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530612"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="5dfeb-103">Tipo de recurso mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="5dfeb-103">mediaContentRatingUnitedKingdom resource type</span></span>

<span data-ttu-id="5dfeb-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5dfeb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5dfeb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5dfeb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5dfeb-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5dfeb-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="5dfeb-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5dfeb-107">Properties</span></span>
|<span data-ttu-id="5dfeb-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5dfeb-108">Property</span></span>|<span data-ttu-id="5dfeb-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5dfeb-109">Type</span></span>|<span data-ttu-id="5dfeb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dfeb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dfeb-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="5dfeb-111">movieRating</span></span>|[<span data-ttu-id="5dfeb-112">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="5dfeb-112">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="5dfeb-113">Classificação de filmes selecionada para o Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="5dfeb-113">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="5dfeb-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="5dfeb-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="5dfeb-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="5dfeb-115">tvRating</span></span>|[<span data-ttu-id="5dfeb-116">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="5dfeb-116">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="5dfeb-117">Classificação de TV selecionada para o Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="5dfeb-117">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="5dfeb-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="5dfeb-118">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5dfeb-119">Relações</span><span class="sxs-lookup"><span data-stu-id="5dfeb-119">Relationships</span></span>
<span data-ttu-id="5dfeb-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5dfeb-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5dfeb-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5dfeb-121">JSON Representation</span></span>
<span data-ttu-id="5dfeb-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5dfeb-122">Here is a JSON representation of the resource.</span></span>
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




