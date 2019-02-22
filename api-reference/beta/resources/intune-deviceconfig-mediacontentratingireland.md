---
title: Tipo de recurso mediaContentRatingIreland
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a17ea1ddbd4e63af846ab6343f66f4a5726e9739
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30140975"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="989c4-103">Tipo de recurso mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="989c4-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="989c4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="989c4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="989c4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="989c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="989c4-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="989c4-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="989c4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="989c4-107">Properties</span></span>
|<span data-ttu-id="989c4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="989c4-108">Property</span></span>|<span data-ttu-id="989c4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="989c4-109">Type</span></span>|<span data-ttu-id="989c4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="989c4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="989c4-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="989c4-111">movieRating</span></span>|[<span data-ttu-id="989c4-112">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="989c4-112">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="989c4-113">Classificação de filmes selecionada para a Irlanda.</span><span class="sxs-lookup"><span data-stu-id="989c4-113">Movies rating selected for Ireland.</span></span> <span data-ttu-id="989c4-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="989c4-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="989c4-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="989c4-115">tvRating</span></span>|[<span data-ttu-id="989c4-116">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="989c4-116">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="989c4-117">Classificação de TV selecionada para a Irlanda.</span><span class="sxs-lookup"><span data-stu-id="989c4-117">TV rating selected for Ireland.</span></span> <span data-ttu-id="989c4-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="989c4-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="989c4-119">Relações</span><span class="sxs-lookup"><span data-stu-id="989c4-119">Relationships</span></span>
<span data-ttu-id="989c4-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="989c4-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="989c4-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="989c4-121">JSON Representation</span></span>
<span data-ttu-id="989c4-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="989c4-122">Here is a JSON representation of the resource.</span></span>
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




