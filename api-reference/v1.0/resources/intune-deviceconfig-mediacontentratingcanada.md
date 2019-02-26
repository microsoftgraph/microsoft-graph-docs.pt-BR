---
title: Tipo de recurso mediaContentRatingCanada
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 88975975b07eb2805ee5f73cc416e3803d5fe24f
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253313"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="b4a86-103">Tipo de recurso mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="b4a86-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="b4a86-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b4a86-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4a86-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b4a86-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b4a86-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b4a86-106">Properties</span></span>
|<span data-ttu-id="b4a86-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4a86-107">Property</span></span>|<span data-ttu-id="b4a86-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4a86-108">Type</span></span>|<span data-ttu-id="b4a86-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4a86-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4a86-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="b4a86-110">movieRating</span></span>|[<span data-ttu-id="b4a86-111">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="b4a86-111">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="b4a86-112">Classificação de filmes selecionada para o Canadá.</span><span class="sxs-lookup"><span data-stu-id="b4a86-112">Movies rating selected for Canada.</span></span> <span data-ttu-id="b4a86-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="b4a86-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="b4a86-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="b4a86-114">tvRating</span></span>|[<span data-ttu-id="b4a86-115">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="b4a86-115">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="b4a86-116">Classificação de TV selecionada para o Canadá.</span><span class="sxs-lookup"><span data-stu-id="b4a86-116">TV rating selected for Canada.</span></span> <span data-ttu-id="b4a86-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="b4a86-117">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4a86-118">Relações</span><span class="sxs-lookup"><span data-stu-id="b4a86-118">Relationships</span></span>
<span data-ttu-id="b4a86-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b4a86-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4a86-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b4a86-120">JSON Representation</span></span>
<span data-ttu-id="b4a86-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b4a86-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingCanada"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingCanada",
  "movieRating": "String",
  "tvRating": "String"
}
```



