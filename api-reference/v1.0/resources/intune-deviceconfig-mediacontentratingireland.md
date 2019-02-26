---
title: Tipo de recurso mediaContentRatingIreland
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 153164010b6beda5d38779f67ffcd0654a1c986a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30252634"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="b7cb8-103">Tipo de recurso mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="b7cb8-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="b7cb8-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b7cb8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7cb8-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b7cb8-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b7cb8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b7cb8-106">Properties</span></span>
|<span data-ttu-id="b7cb8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7cb8-107">Property</span></span>|<span data-ttu-id="b7cb8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7cb8-108">Type</span></span>|<span data-ttu-id="b7cb8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7cb8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7cb8-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="b7cb8-110">movieRating</span></span>|[<span data-ttu-id="b7cb8-111">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="b7cb8-111">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="b7cb8-112">Classificação de filmes selecionada para a Irlanda.</span><span class="sxs-lookup"><span data-stu-id="b7cb8-112">Movies rating selected for Ireland.</span></span> <span data-ttu-id="b7cb8-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="b7cb8-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="b7cb8-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="b7cb8-114">tvRating</span></span>|[<span data-ttu-id="b7cb8-115">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="b7cb8-115">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="b7cb8-116">Classificação de TV selecionada para a Irlanda.</span><span class="sxs-lookup"><span data-stu-id="b7cb8-116">TV rating selected for Ireland.</span></span> <span data-ttu-id="b7cb8-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="b7cb8-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7cb8-118">Relações</span><span class="sxs-lookup"><span data-stu-id="b7cb8-118">Relationships</span></span>
<span data-ttu-id="b7cb8-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b7cb8-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7cb8-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b7cb8-120">JSON Representation</span></span>
<span data-ttu-id="b7cb8-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b7cb8-121">Here is a JSON representation of the resource.</span></span>
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



