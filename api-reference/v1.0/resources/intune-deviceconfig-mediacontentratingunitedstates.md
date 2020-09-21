---
title: Tipo de recurso mediaContentRatingUnitedStates
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 30e41727b84e7f10b82917f4dc1dd23f296cc19f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003056"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="a00be-103">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="a00be-103">mediaContentRatingUnitedStates resource type</span></span>

<span data-ttu-id="a00be-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a00be-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a00be-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a00be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a00be-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a00be-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a00be-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a00be-107">Properties</span></span>
|<span data-ttu-id="a00be-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a00be-108">Property</span></span>|<span data-ttu-id="a00be-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a00be-109">Type</span></span>|<span data-ttu-id="a00be-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a00be-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a00be-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="a00be-111">movieRating</span></span>|[<span data-ttu-id="a00be-112">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="a00be-112">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="a00be-113">Classificação de filmes selecionada para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="a00be-113">Movies rating selected for United States.</span></span> <span data-ttu-id="a00be-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="a00be-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="a00be-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="a00be-115">tvRating</span></span>|[<span data-ttu-id="a00be-116">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="a00be-116">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="a00be-117">Classificação de TV selecionada para Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="a00be-117">TV rating selected for United States.</span></span> <span data-ttu-id="a00be-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="a00be-118">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a00be-119">Relações</span><span class="sxs-lookup"><span data-stu-id="a00be-119">Relationships</span></span>
<span data-ttu-id="a00be-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a00be-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a00be-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a00be-121">JSON Representation</span></span>
<span data-ttu-id="a00be-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a00be-122">Here is a JSON representation of the resource.</span></span>
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









