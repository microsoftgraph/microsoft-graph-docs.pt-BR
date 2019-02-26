---
title: Tipo de recurso mediaContentRatingGermany
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e3c59bf110c55492db49a81a557cef0b421e328
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260351"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="db057-103">Tipo de recurso mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="db057-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="db057-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="db057-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db057-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="db057-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="db057-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="db057-106">Properties</span></span>
|<span data-ttu-id="db057-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db057-107">Property</span></span>|<span data-ttu-id="db057-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="db057-108">Type</span></span>|<span data-ttu-id="db057-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="db057-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db057-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="db057-110">movieRating</span></span>|[<span data-ttu-id="db057-111">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="db057-111">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="db057-112">Classificação de filmes selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="db057-112">Movies rating selected for Germany.</span></span> <span data-ttu-id="db057-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="db057-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="db057-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="db057-114">tvRating</span></span>|[<span data-ttu-id="db057-115">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="db057-115">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="db057-116">Classificação de TV selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="db057-116">TV rating selected for Germany.</span></span> <span data-ttu-id="db057-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="db057-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db057-118">Relações</span><span class="sxs-lookup"><span data-stu-id="db057-118">Relationships</span></span>
<span data-ttu-id="db057-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="db057-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="db057-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="db057-120">JSON Representation</span></span>
<span data-ttu-id="db057-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="db057-121">Here is a JSON representation of the resource.</span></span>
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



