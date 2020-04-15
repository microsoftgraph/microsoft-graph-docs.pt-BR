---
title: Tipo de recurso mediaContentRatingIreland
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 01135bb6c5a19ae837a834a51a5857b5f54baac0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473157"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="a7da1-103">Tipo de recurso mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="a7da1-103">mediaContentRatingIreland resource type</span></span>

<span data-ttu-id="a7da1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7da1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a7da1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a7da1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7da1-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a7da1-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a7da1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a7da1-107">Properties</span></span>
|<span data-ttu-id="a7da1-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7da1-108">Property</span></span>|<span data-ttu-id="a7da1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7da1-109">Type</span></span>|<span data-ttu-id="a7da1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7da1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7da1-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="a7da1-111">movieRating</span></span>|[<span data-ttu-id="a7da1-112">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="a7da1-112">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="a7da1-113">Classificação de filmes selecionada para a Irlanda.</span><span class="sxs-lookup"><span data-stu-id="a7da1-113">Movies rating selected for Ireland.</span></span> <span data-ttu-id="a7da1-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="a7da1-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="a7da1-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="a7da1-115">tvRating</span></span>|[<span data-ttu-id="a7da1-116">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="a7da1-116">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="a7da1-117">Classificação de TV selecionada para a Irlanda.</span><span class="sxs-lookup"><span data-stu-id="a7da1-117">TV rating selected for Ireland.</span></span> <span data-ttu-id="a7da1-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="a7da1-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7da1-119">Relações</span><span class="sxs-lookup"><span data-stu-id="a7da1-119">Relationships</span></span>
<span data-ttu-id="a7da1-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a7da1-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7da1-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a7da1-121">JSON Representation</span></span>
<span data-ttu-id="a7da1-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a7da1-122">Here is a JSON representation of the resource.</span></span>
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







