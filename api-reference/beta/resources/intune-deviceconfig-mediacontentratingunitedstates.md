---
title: Tipo de recurso mediaContentRatingUnitedStates
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 130b74fa3cf0a5424f7ad816107b80101b9cee49
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161898"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="5c42e-103">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="5c42e-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="5c42e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5c42e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5c42e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5c42e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c42e-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5c42e-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="5c42e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5c42e-107">Properties</span></span>
|<span data-ttu-id="5c42e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5c42e-108">Property</span></span>|<span data-ttu-id="5c42e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5c42e-109">Type</span></span>|<span data-ttu-id="5c42e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5c42e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c42e-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="5c42e-111">movieRating</span></span>|[<span data-ttu-id="5c42e-112">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="5c42e-112">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="5c42e-113">Classificação de filmes selecionada para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="5c42e-113">Movies rating selected for United States.</span></span> <span data-ttu-id="5c42e-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="5c42e-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="5c42e-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="5c42e-115">tvRating</span></span>|[<span data-ttu-id="5c42e-116">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="5c42e-116">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="5c42e-117">Classificação de TV selecionada para Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="5c42e-117">TV rating selected for United States.</span></span> <span data-ttu-id="5c42e-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="5c42e-118">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c42e-119">Relações</span><span class="sxs-lookup"><span data-stu-id="5c42e-119">Relationships</span></span>
<span data-ttu-id="5c42e-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5c42e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c42e-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5c42e-121">JSON Representation</span></span>
<span data-ttu-id="5c42e-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5c42e-122">Here is a JSON representation of the resource.</span></span>
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




