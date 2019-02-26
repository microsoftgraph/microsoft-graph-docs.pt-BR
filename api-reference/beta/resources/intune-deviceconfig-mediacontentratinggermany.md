---
title: Tipo de recurso mediaContentRatingGermany
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a43f919bb24d25d0e22dab0ecc192b2b6757f9e7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147093"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="43e82-103">Tipo de recurso mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="43e82-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="43e82-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="43e82-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43e82-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="43e82-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43e82-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="43e82-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="43e82-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="43e82-107">Properties</span></span>
|<span data-ttu-id="43e82-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43e82-108">Property</span></span>|<span data-ttu-id="43e82-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="43e82-109">Type</span></span>|<span data-ttu-id="43e82-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="43e82-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43e82-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="43e82-111">movieRating</span></span>|[<span data-ttu-id="43e82-112">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="43e82-112">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="43e82-113">Classificação de filmes selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="43e82-113">Movies rating selected for Germany.</span></span> <span data-ttu-id="43e82-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="43e82-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="43e82-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="43e82-115">tvRating</span></span>|[<span data-ttu-id="43e82-116">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="43e82-116">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="43e82-117">Classificação de TV selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="43e82-117">TV rating selected for Germany.</span></span> <span data-ttu-id="43e82-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="43e82-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43e82-119">Relações</span><span class="sxs-lookup"><span data-stu-id="43e82-119">Relationships</span></span>
<span data-ttu-id="43e82-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="43e82-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="43e82-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="43e82-121">JSON Representation</span></span>
<span data-ttu-id="43e82-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="43e82-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```




