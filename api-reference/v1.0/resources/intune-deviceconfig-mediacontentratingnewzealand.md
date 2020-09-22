---
title: Tipo de recurso mediaContentRatingNewZealand
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2860f308cb25b679ea12b2b2d978cf15dc87c40a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003091"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="1176f-103">Tipo de recurso mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="1176f-103">mediaContentRatingNewZealand resource type</span></span>

<span data-ttu-id="1176f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1176f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1176f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1176f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1176f-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1176f-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1176f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1176f-107">Properties</span></span>
|<span data-ttu-id="1176f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1176f-108">Property</span></span>|<span data-ttu-id="1176f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1176f-109">Type</span></span>|<span data-ttu-id="1176f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1176f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1176f-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="1176f-111">movieRating</span></span>|[<span data-ttu-id="1176f-112">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="1176f-112">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="1176f-113">Classificação de filmes selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="1176f-113">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="1176f-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="1176f-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="1176f-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="1176f-115">tvRating</span></span>|[<span data-ttu-id="1176f-116">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="1176f-116">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="1176f-117">Classificação de TV selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="1176f-117">TV rating selected for New Zealand.</span></span> <span data-ttu-id="1176f-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="1176f-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1176f-119">Relações</span><span class="sxs-lookup"><span data-stu-id="1176f-119">Relationships</span></span>
<span data-ttu-id="1176f-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1176f-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1176f-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1176f-121">JSON Representation</span></span>
<span data-ttu-id="1176f-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1176f-122">Here is a JSON representation of the resource.</span></span>
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









