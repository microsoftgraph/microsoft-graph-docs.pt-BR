---
title: Tipo de recurso mediaContentRatingUnitedKingdom
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5e9fd03ebd0834ff63c129216833673255715f76
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003084"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="23691-103">Tipo de recurso mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="23691-103">mediaContentRatingUnitedKingdom resource type</span></span>

<span data-ttu-id="23691-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23691-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23691-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="23691-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23691-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="23691-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="23691-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23691-107">Properties</span></span>
|<span data-ttu-id="23691-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23691-108">Property</span></span>|<span data-ttu-id="23691-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="23691-109">Type</span></span>|<span data-ttu-id="23691-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="23691-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23691-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="23691-111">movieRating</span></span>|[<span data-ttu-id="23691-112">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="23691-112">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="23691-113">Classificação de filmes selecionada para o Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="23691-113">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="23691-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="23691-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="23691-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="23691-115">tvRating</span></span>|[<span data-ttu-id="23691-116">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="23691-116">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="23691-117">Classificação de TV selecionada para o Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="23691-117">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="23691-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="23691-118">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23691-119">Relações</span><span class="sxs-lookup"><span data-stu-id="23691-119">Relationships</span></span>
<span data-ttu-id="23691-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23691-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23691-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23691-121">JSON Representation</span></span>
<span data-ttu-id="23691-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23691-122">Here is a JSON representation of the resource.</span></span>
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









