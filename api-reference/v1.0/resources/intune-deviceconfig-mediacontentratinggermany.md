---
title: Tipo de recurso mediaContentRatingGermany
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b4f2eda6b9666d3b23ea48d96f7a7231e189b4f5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028095"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="9d205-103">Tipo de recurso mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="9d205-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="9d205-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9d205-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d205-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9d205-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9d205-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d205-106">Properties</span></span>
|<span data-ttu-id="9d205-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d205-107">Property</span></span>|<span data-ttu-id="9d205-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d205-108">Type</span></span>|<span data-ttu-id="9d205-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d205-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d205-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="9d205-110">movieRating</span></span>|[<span data-ttu-id="9d205-111">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="9d205-111">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="9d205-112">Classificação de filmes selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="9d205-112">Movies rating selected for Germany.</span></span> <span data-ttu-id="9d205-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="9d205-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="9d205-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="9d205-114">tvRating</span></span>|[<span data-ttu-id="9d205-115">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="9d205-115">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="9d205-116">Classificação de TV selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="9d205-116">TV rating selected for Germany.</span></span> <span data-ttu-id="9d205-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="9d205-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d205-118">Relações</span><span class="sxs-lookup"><span data-stu-id="9d205-118">Relationships</span></span>
<span data-ttu-id="9d205-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9d205-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d205-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d205-120">JSON Representation</span></span>
<span data-ttu-id="9d205-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9d205-121">Here is a JSON representation of the resource.</span></span>
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



