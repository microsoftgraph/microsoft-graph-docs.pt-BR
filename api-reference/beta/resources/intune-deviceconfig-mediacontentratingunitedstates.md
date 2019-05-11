---
title: Tipo de recurso mediaContentRatingUnitedStates
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f085bc24c3c5bd7b510ee5fa0a0b841361c0269e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950757"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="ae6a2-103">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="ae6a2-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="ae6a2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ae6a2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae6a2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ae6a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae6a2-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ae6a2-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ae6a2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ae6a2-107">Properties</span></span>
|<span data-ttu-id="ae6a2-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ae6a2-108">Property</span></span>|<span data-ttu-id="ae6a2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae6a2-109">Type</span></span>|<span data-ttu-id="ae6a2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae6a2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae6a2-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="ae6a2-111">movieRating</span></span>|[<span data-ttu-id="ae6a2-112">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="ae6a2-112">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="ae6a2-113">Classificação de filmes selecionada para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="ae6a2-113">Movies rating selected for United States.</span></span> <span data-ttu-id="ae6a2-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="ae6a2-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="ae6a2-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="ae6a2-115">tvRating</span></span>|[<span data-ttu-id="ae6a2-116">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="ae6a2-116">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="ae6a2-117">Classificação de TV selecionada para Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="ae6a2-117">TV rating selected for United States.</span></span> <span data-ttu-id="ae6a2-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="ae6a2-118">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae6a2-119">Relações</span><span class="sxs-lookup"><span data-stu-id="ae6a2-119">Relationships</span></span>
<span data-ttu-id="ae6a2-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ae6a2-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae6a2-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ae6a2-121">JSON Representation</span></span>
<span data-ttu-id="ae6a2-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ae6a2-122">Here is a JSON representation of the resource.</span></span>
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




