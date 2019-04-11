---
title: Tipo de recurso mediaContentRatingFrance
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e3d270bfb876f33afdd1944f070aaefe58fe569
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31786781"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="eca48-103">Tipo de recurso mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="eca48-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="eca48-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eca48-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eca48-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eca48-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eca48-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="eca48-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="eca48-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eca48-107">Properties</span></span>
|<span data-ttu-id="eca48-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eca48-108">Property</span></span>|<span data-ttu-id="eca48-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="eca48-109">Type</span></span>|<span data-ttu-id="eca48-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="eca48-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eca48-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="eca48-111">movieRating</span></span>|[<span data-ttu-id="eca48-112">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="eca48-112">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="eca48-113">Classificação de filmes selecionada para a França.</span><span class="sxs-lookup"><span data-stu-id="eca48-113">Movies rating selected for France.</span></span> <span data-ttu-id="eca48-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="eca48-114">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="eca48-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="eca48-115">tvRating</span></span>|[<span data-ttu-id="eca48-116">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="eca48-116">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="eca48-117">Classificação de TV selecionada para a França.</span><span class="sxs-lookup"><span data-stu-id="eca48-117">TV rating selected for France.</span></span> <span data-ttu-id="eca48-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="eca48-118">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eca48-119">Relações</span><span class="sxs-lookup"><span data-stu-id="eca48-119">Relationships</span></span>
<span data-ttu-id="eca48-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="eca48-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eca48-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eca48-121">JSON Representation</span></span>
<span data-ttu-id="eca48-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eca48-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```





