---
title: Tipo de recurso mediaContentRatingFrance
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2babce1e41f855d17b7c1b39e3d89dc56f669ebb
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34980401"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="f01ee-103">Tipo de recurso mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="f01ee-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="f01ee-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f01ee-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f01ee-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f01ee-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f01ee-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f01ee-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f01ee-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f01ee-107">Properties</span></span>
|<span data-ttu-id="f01ee-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f01ee-108">Property</span></span>|<span data-ttu-id="f01ee-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f01ee-109">Type</span></span>|<span data-ttu-id="f01ee-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f01ee-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f01ee-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="f01ee-111">movieRating</span></span>|[<span data-ttu-id="f01ee-112">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="f01ee-112">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="f01ee-113">Classificação de filmes selecionada para a França.</span><span class="sxs-lookup"><span data-stu-id="f01ee-113">Movies rating selected for France.</span></span> <span data-ttu-id="f01ee-114">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="f01ee-114">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="f01ee-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="f01ee-115">tvRating</span></span>|[<span data-ttu-id="f01ee-116">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="f01ee-116">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="f01ee-117">Classificação de TV selecionada para a França.</span><span class="sxs-lookup"><span data-stu-id="f01ee-117">TV rating selected for France.</span></span> <span data-ttu-id="f01ee-118">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="f01ee-118">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f01ee-119">Relações</span><span class="sxs-lookup"><span data-stu-id="f01ee-119">Relationships</span></span>
<span data-ttu-id="f01ee-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f01ee-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f01ee-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f01ee-121">JSON Representation</span></span>
<span data-ttu-id="f01ee-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f01ee-122">Here is a JSON representation of the resource.</span></span>
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





