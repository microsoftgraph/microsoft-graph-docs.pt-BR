---
title: Tipo de recurso mediaContentRatingUnitedStates
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0175f6f0894df0c859f9951f43c3bb4b857a2256
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760005"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="216ac-103">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="216ac-103">mediaContentRatingUnitedStates resource type</span></span>

<span data-ttu-id="216ac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="216ac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="216ac-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="216ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="216ac-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="216ac-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="216ac-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="216ac-107">Properties</span></span>
|<span data-ttu-id="216ac-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="216ac-108">Property</span></span>|<span data-ttu-id="216ac-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="216ac-109">Type</span></span>|<span data-ttu-id="216ac-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="216ac-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="216ac-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="216ac-111">movieRating</span></span>|[<span data-ttu-id="216ac-112">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="216ac-112">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="216ac-113">Classificação de filmes selecionada para Os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="216ac-113">Movies rating selected for United States.</span></span> <span data-ttu-id="216ac-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="216ac-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="216ac-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="216ac-115">tvRating</span></span>|[<span data-ttu-id="216ac-116">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="216ac-116">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="216ac-117">Classificação de TV selecionada para Os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="216ac-117">TV rating selected for United States.</span></span> <span data-ttu-id="216ac-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="216ac-118">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="216ac-119">Relações</span><span class="sxs-lookup"><span data-stu-id="216ac-119">Relationships</span></span>
<span data-ttu-id="216ac-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="216ac-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="216ac-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="216ac-121">JSON Representation</span></span>
<span data-ttu-id="216ac-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="216ac-122">Here is a JSON representation of the resource.</span></span>
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




