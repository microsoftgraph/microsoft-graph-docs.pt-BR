---
title: Tipo de recurso mediaContentRatingIreland
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dc67f39a0cbb42dc42d942bd17387ba1f4e99fd6
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530625"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="199b9-103">Tipo de recurso mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="199b9-103">mediaContentRatingIreland resource type</span></span>

<span data-ttu-id="199b9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="199b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="199b9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="199b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="199b9-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="199b9-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="199b9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="199b9-107">Properties</span></span>
|<span data-ttu-id="199b9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="199b9-108">Property</span></span>|<span data-ttu-id="199b9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="199b9-109">Type</span></span>|<span data-ttu-id="199b9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="199b9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="199b9-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="199b9-111">movieRating</span></span>|[<span data-ttu-id="199b9-112">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="199b9-112">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="199b9-113">Classificação de filmes selecionada para a Irlanda.</span><span class="sxs-lookup"><span data-stu-id="199b9-113">Movies rating selected for Ireland.</span></span> <span data-ttu-id="199b9-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="199b9-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="199b9-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="199b9-115">tvRating</span></span>|[<span data-ttu-id="199b9-116">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="199b9-116">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="199b9-117">Classificação de TV selecionada para a Irlanda.</span><span class="sxs-lookup"><span data-stu-id="199b9-117">TV rating selected for Ireland.</span></span> <span data-ttu-id="199b9-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="199b9-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="199b9-119">Relações</span><span class="sxs-lookup"><span data-stu-id="199b9-119">Relationships</span></span>
<span data-ttu-id="199b9-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="199b9-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="199b9-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="199b9-121">JSON Representation</span></span>
<span data-ttu-id="199b9-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="199b9-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```




