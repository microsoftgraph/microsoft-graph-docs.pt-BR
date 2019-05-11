---
title: Tipo de recurso mediaContentRatingNewZealand
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 48698cf0f35fc39c8e385d391344914ea34745ea
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950876"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="622d3-103">Tipo de recurso mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="622d3-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="622d3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="622d3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="622d3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="622d3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="622d3-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="622d3-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="622d3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="622d3-107">Properties</span></span>
|<span data-ttu-id="622d3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="622d3-108">Property</span></span>|<span data-ttu-id="622d3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="622d3-109">Type</span></span>|<span data-ttu-id="622d3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="622d3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="622d3-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="622d3-111">movieRating</span></span>|[<span data-ttu-id="622d3-112">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="622d3-112">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="622d3-113">Classificação de filmes selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="622d3-113">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="622d3-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="622d3-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="622d3-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="622d3-115">tvRating</span></span>|[<span data-ttu-id="622d3-116">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="622d3-116">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="622d3-117">Classificação de TV selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="622d3-117">TV rating selected for New Zealand.</span></span> <span data-ttu-id="622d3-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="622d3-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="622d3-119">Relações</span><span class="sxs-lookup"><span data-stu-id="622d3-119">Relationships</span></span>
<span data-ttu-id="622d3-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="622d3-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="622d3-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="622d3-121">JSON Representation</span></span>
<span data-ttu-id="622d3-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="622d3-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```




