---
title: Tipo de recurso mediaContentRatingNewZealand
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9328ccc8b3c6b7ce6af220d8f798497e00448a8b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159273"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="3c8ed-103">Tipo de recurso mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="3c8ed-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="3c8ed-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3c8ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c8ed-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3c8ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c8ed-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3c8ed-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="3c8ed-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3c8ed-107">Properties</span></span>
|<span data-ttu-id="3c8ed-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c8ed-108">Property</span></span>|<span data-ttu-id="3c8ed-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c8ed-109">Type</span></span>|<span data-ttu-id="3c8ed-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c8ed-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c8ed-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="3c8ed-111">movieRating</span></span>|[<span data-ttu-id="3c8ed-112">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="3c8ed-112">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="3c8ed-113">Classificação de filmes selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="3c8ed-113">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="3c8ed-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="3c8ed-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="3c8ed-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="3c8ed-115">tvRating</span></span>|[<span data-ttu-id="3c8ed-116">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="3c8ed-116">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="3c8ed-117">Classificação de TV selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="3c8ed-117">TV rating selected for New Zealand.</span></span> <span data-ttu-id="3c8ed-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="3c8ed-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c8ed-119">Relações</span><span class="sxs-lookup"><span data-stu-id="3c8ed-119">Relationships</span></span>
<span data-ttu-id="3c8ed-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3c8ed-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c8ed-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c8ed-121">JSON Representation</span></span>
<span data-ttu-id="3c8ed-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3c8ed-122">Here is a JSON representation of the resource.</span></span>
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




