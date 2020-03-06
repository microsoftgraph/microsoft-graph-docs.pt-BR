---
title: Tipo de recurso mediaContentRatingUnitedStates
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c5ed2470ff226a5c593dfed892bafb7b0fc3431d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532437"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="f08c3-103">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="f08c3-103">mediaContentRatingUnitedStates resource type</span></span>

<span data-ttu-id="f08c3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f08c3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f08c3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f08c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f08c3-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f08c3-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f08c3-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f08c3-107">Properties</span></span>
|<span data-ttu-id="f08c3-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f08c3-108">Property</span></span>|<span data-ttu-id="f08c3-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f08c3-109">Type</span></span>|<span data-ttu-id="f08c3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f08c3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f08c3-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="f08c3-111">movieRating</span></span>|[<span data-ttu-id="f08c3-112">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="f08c3-112">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="f08c3-113">Classificação de filmes selecionada para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="f08c3-113">Movies rating selected for United States.</span></span> <span data-ttu-id="f08c3-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="f08c3-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="f08c3-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="f08c3-115">tvRating</span></span>|[<span data-ttu-id="f08c3-116">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="f08c3-116">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="f08c3-117">Classificação de TV selecionada para Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="f08c3-117">TV rating selected for United States.</span></span> <span data-ttu-id="f08c3-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="f08c3-118">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f08c3-119">Relações</span><span class="sxs-lookup"><span data-stu-id="f08c3-119">Relationships</span></span>
<span data-ttu-id="f08c3-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f08c3-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f08c3-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f08c3-121">JSON Representation</span></span>
<span data-ttu-id="f08c3-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f08c3-122">Here is a JSON representation of the resource.</span></span>
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




