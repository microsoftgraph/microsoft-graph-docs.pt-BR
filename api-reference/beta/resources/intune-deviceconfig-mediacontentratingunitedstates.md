---
title: Tipo de recurso mediaContentRatingUnitedStates
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6bc4383dd9207be3c6142857b1a6b938d7cc5b60
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273450"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="e3153-103">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="e3153-103">mediaContentRatingUnitedStates resource type</span></span>

<span data-ttu-id="e3153-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3153-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3153-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e3153-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3153-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e3153-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3153-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e3153-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e3153-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3153-108">Properties</span></span>
|<span data-ttu-id="e3153-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3153-109">Property</span></span>|<span data-ttu-id="e3153-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3153-110">Type</span></span>|<span data-ttu-id="e3153-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3153-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3153-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="e3153-112">movieRating</span></span>|[<span data-ttu-id="e3153-113">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="e3153-113">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="e3153-114">Classificação de filmes selecionada para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="e3153-114">Movies rating selected for United States.</span></span> <span data-ttu-id="e3153-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="e3153-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="e3153-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="e3153-116">tvRating</span></span>|[<span data-ttu-id="e3153-117">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="e3153-117">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="e3153-118">Classificação de TV selecionada para Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="e3153-118">TV rating selected for United States.</span></span> <span data-ttu-id="e3153-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="e3153-119">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3153-120">Relações</span><span class="sxs-lookup"><span data-stu-id="e3153-120">Relationships</span></span>
<span data-ttu-id="e3153-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e3153-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3153-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3153-122">JSON Representation</span></span>
<span data-ttu-id="e3153-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e3153-123">Here is a JSON representation of the resource.</span></span>
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




