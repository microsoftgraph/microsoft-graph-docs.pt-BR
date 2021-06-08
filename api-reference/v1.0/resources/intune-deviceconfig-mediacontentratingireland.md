---
title: Tipo de recurso mediaContentRatingIreland
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cb96a239ff31a0d6843b690d063361a65099e65e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760019"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="72265-103">Tipo de recurso mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="72265-103">mediaContentRatingIreland resource type</span></span>

<span data-ttu-id="72265-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72265-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72265-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="72265-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72265-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="72265-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="72265-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="72265-107">Properties</span></span>
|<span data-ttu-id="72265-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="72265-108">Property</span></span>|<span data-ttu-id="72265-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="72265-109">Type</span></span>|<span data-ttu-id="72265-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="72265-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72265-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="72265-111">movieRating</span></span>|[<span data-ttu-id="72265-112">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="72265-112">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="72265-113">Classificação de filmes selecionada para a Irlanda.</span><span class="sxs-lookup"><span data-stu-id="72265-113">Movies rating selected for Ireland.</span></span> <span data-ttu-id="72265-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="72265-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="72265-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="72265-115">tvRating</span></span>|[<span data-ttu-id="72265-116">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="72265-116">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="72265-117">Classificação de TV selecionada para a Irlanda.</span><span class="sxs-lookup"><span data-stu-id="72265-117">TV rating selected for Ireland.</span></span> <span data-ttu-id="72265-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="72265-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72265-119">Relações</span><span class="sxs-lookup"><span data-stu-id="72265-119">Relationships</span></span>
<span data-ttu-id="72265-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="72265-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="72265-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="72265-121">JSON Representation</span></span>
<span data-ttu-id="72265-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="72265-122">Here is a JSON representation of the resource.</span></span>
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




