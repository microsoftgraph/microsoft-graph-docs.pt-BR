---
title: Tipo de recurso mediaContentRatingUnitedStates
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c6c6df674fc4cef174892d4cdb27303c3933fcdd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031371"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="a77c8-103">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="a77c8-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="a77c8-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a77c8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a77c8-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a77c8-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a77c8-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a77c8-106">Properties</span></span>
|<span data-ttu-id="a77c8-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a77c8-107">Property</span></span>|<span data-ttu-id="a77c8-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a77c8-108">Type</span></span>|<span data-ttu-id="a77c8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a77c8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a77c8-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="a77c8-110">movieRating</span></span>|[<span data-ttu-id="a77c8-111">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="a77c8-111">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="a77c8-112">Classificação de filmes selecionada para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="a77c8-112">Movies rating selected for United States.</span></span> <span data-ttu-id="a77c8-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="a77c8-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="a77c8-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="a77c8-114">tvRating</span></span>|[<span data-ttu-id="a77c8-115">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="a77c8-115">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="a77c8-116">Classificação de TV selecionada para Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="a77c8-116">TV rating selected for United States.</span></span> <span data-ttu-id="a77c8-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="a77c8-117">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a77c8-118">Relações</span><span class="sxs-lookup"><span data-stu-id="a77c8-118">Relationships</span></span>
<span data-ttu-id="a77c8-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a77c8-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a77c8-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a77c8-120">JSON Representation</span></span>
<span data-ttu-id="a77c8-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a77c8-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```



