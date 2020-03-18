---
title: Tipo de recurso mediaContentRatingUnitedStates
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 59029a86d21cc0f185f66222b054618cb34977cd
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788545"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="db7ea-103">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="db7ea-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="db7ea-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="db7ea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="db7ea-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="db7ea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db7ea-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="db7ea-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="db7ea-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="db7ea-107">Properties</span></span>
|<span data-ttu-id="db7ea-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="db7ea-108">Property</span></span>|<span data-ttu-id="db7ea-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="db7ea-109">Type</span></span>|<span data-ttu-id="db7ea-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="db7ea-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db7ea-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="db7ea-111">movieRating</span></span>|[<span data-ttu-id="db7ea-112">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="db7ea-112">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="db7ea-113">Classificação de filmes selecionada para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="db7ea-113">Movies rating selected for United States.</span></span> <span data-ttu-id="db7ea-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="db7ea-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="db7ea-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="db7ea-115">tvRating</span></span>|[<span data-ttu-id="db7ea-116">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="db7ea-116">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="db7ea-117">Classificação de TV selecionada para Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="db7ea-117">TV rating selected for United States.</span></span> <span data-ttu-id="db7ea-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="db7ea-118">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db7ea-119">Relações</span><span class="sxs-lookup"><span data-stu-id="db7ea-119">Relationships</span></span>
<span data-ttu-id="db7ea-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="db7ea-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="db7ea-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="db7ea-121">JSON Representation</span></span>
<span data-ttu-id="db7ea-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="db7ea-122">Here is a JSON representation of the resource.</span></span>
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



