---
title: Tipo de recurso mediaContentRatingCanada
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9735497f3f2f71f28b8fe9847d2664bd4e65e959
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028109"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="5ab7b-103">Tipo de recurso mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="5ab7b-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="5ab7b-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5ab7b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ab7b-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5ab7b-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="5ab7b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5ab7b-106">Properties</span></span>
|<span data-ttu-id="5ab7b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ab7b-107">Property</span></span>|<span data-ttu-id="5ab7b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ab7b-108">Type</span></span>|<span data-ttu-id="5ab7b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ab7b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ab7b-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="5ab7b-110">movieRating</span></span>|[<span data-ttu-id="5ab7b-111">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="5ab7b-111">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="5ab7b-112">Classificação de filmes selecionada para o Canadá.</span><span class="sxs-lookup"><span data-stu-id="5ab7b-112">Movies rating selected for Canada.</span></span> <span data-ttu-id="5ab7b-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="5ab7b-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="5ab7b-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="5ab7b-114">tvRating</span></span>|[<span data-ttu-id="5ab7b-115">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="5ab7b-115">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="5ab7b-116">Classificação de TV selecionada para o Canadá.</span><span class="sxs-lookup"><span data-stu-id="5ab7b-116">TV rating selected for Canada.</span></span> <span data-ttu-id="5ab7b-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="5ab7b-117">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ab7b-118">Relações</span><span class="sxs-lookup"><span data-stu-id="5ab7b-118">Relationships</span></span>
<span data-ttu-id="5ab7b-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5ab7b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ab7b-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5ab7b-120">JSON Representation</span></span>
<span data-ttu-id="5ab7b-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5ab7b-121">Here is a JSON representation of the resource.</span></span>
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



