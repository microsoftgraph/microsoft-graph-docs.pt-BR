---
title: Tipo de recurso mediaContentRatingNewZealand
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9d06658905a5a6e5aaab79bb159a87fe4cb5cf7a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031392"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="42994-103">Tipo de recurso mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="42994-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="42994-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="42994-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42994-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="42994-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="42994-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="42994-106">Properties</span></span>
|<span data-ttu-id="42994-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="42994-107">Property</span></span>|<span data-ttu-id="42994-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="42994-108">Type</span></span>|<span data-ttu-id="42994-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="42994-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42994-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="42994-110">movieRating</span></span>|[<span data-ttu-id="42994-111">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="42994-111">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="42994-112">Classificação de filmes selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="42994-112">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="42994-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="42994-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="42994-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="42994-114">tvRating</span></span>|[<span data-ttu-id="42994-115">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="42994-115">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="42994-116">Classificação de TV selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="42994-116">TV rating selected for New Zealand.</span></span> <span data-ttu-id="42994-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="42994-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42994-118">Relações</span><span class="sxs-lookup"><span data-stu-id="42994-118">Relationships</span></span>
<span data-ttu-id="42994-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="42994-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="42994-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="42994-120">JSON Representation</span></span>
<span data-ttu-id="42994-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="42994-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```



