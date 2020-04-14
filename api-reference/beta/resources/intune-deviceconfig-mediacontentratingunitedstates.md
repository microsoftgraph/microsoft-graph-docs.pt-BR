---
title: Tipo de recurso mediaContentRatingUnitedStates
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 570a79280762af3977f88cf374a994a45dfaee4e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437137"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="4a560-103">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="4a560-103">mediaContentRatingUnitedStates resource type</span></span>

<span data-ttu-id="4a560-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a560-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4a560-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4a560-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a560-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4a560-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a560-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4a560-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="4a560-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a560-108">Properties</span></span>
|<span data-ttu-id="4a560-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a560-109">Property</span></span>|<span data-ttu-id="4a560-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a560-110">Type</span></span>|<span data-ttu-id="4a560-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a560-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a560-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="4a560-112">movieRating</span></span>|[<span data-ttu-id="4a560-113">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="4a560-113">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="4a560-114">Classificação de filmes selecionada para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="4a560-114">Movies rating selected for United States.</span></span> <span data-ttu-id="4a560-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="4a560-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="4a560-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="4a560-116">tvRating</span></span>|[<span data-ttu-id="4a560-117">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="4a560-117">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="4a560-118">Classificação de TV selecionada para Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="4a560-118">TV rating selected for United States.</span></span> <span data-ttu-id="4a560-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="4a560-119">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a560-120">Relações</span><span class="sxs-lookup"><span data-stu-id="4a560-120">Relationships</span></span>
<span data-ttu-id="4a560-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4a560-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a560-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a560-122">JSON Representation</span></span>
<span data-ttu-id="4a560-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4a560-123">Here is a JSON representation of the resource.</span></span>
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



