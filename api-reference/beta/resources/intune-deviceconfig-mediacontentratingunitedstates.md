---
title: Tipo de recurso mediaContentRatingUnitedStates
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 60208f2bace4826f06ff5a81f02bc087211d52a1
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31777897"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="7bfce-103">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="7bfce-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="7bfce-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7bfce-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7bfce-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7bfce-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bfce-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7bfce-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="7bfce-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7bfce-107">Properties</span></span>
|<span data-ttu-id="7bfce-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7bfce-108">Property</span></span>|<span data-ttu-id="7bfce-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7bfce-109">Type</span></span>|<span data-ttu-id="7bfce-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7bfce-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bfce-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="7bfce-111">movieRating</span></span>|[<span data-ttu-id="7bfce-112">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="7bfce-112">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="7bfce-113">Classificação de filmes selecionada para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="7bfce-113">Movies rating selected for United States.</span></span> <span data-ttu-id="7bfce-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="7bfce-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="7bfce-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="7bfce-115">tvRating</span></span>|[<span data-ttu-id="7bfce-116">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="7bfce-116">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="7bfce-117">Classificação de TV selecionada para Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="7bfce-117">TV rating selected for United States.</span></span> <span data-ttu-id="7bfce-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="7bfce-118">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bfce-119">Relações</span><span class="sxs-lookup"><span data-stu-id="7bfce-119">Relationships</span></span>
<span data-ttu-id="7bfce-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="7bfce-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7bfce-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7bfce-121">JSON Representation</span></span>
<span data-ttu-id="7bfce-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7bfce-122">Here is a JSON representation of the resource.</span></span>
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





