---
title: Tipo de recurso mediaContentRatingUnitedStates
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: baa5d98f0fcb1d267221c95c0b27be988d3a197f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572315"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="57e68-103">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="57e68-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="57e68-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="57e68-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57e68-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="57e68-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="57e68-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="57e68-106">Properties</span></span>
|<span data-ttu-id="57e68-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57e68-107">Property</span></span>|<span data-ttu-id="57e68-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="57e68-108">Type</span></span>|<span data-ttu-id="57e68-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="57e68-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57e68-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="57e68-110">movieRating</span></span>|[<span data-ttu-id="57e68-111">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="57e68-111">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="57e68-112">Classificação de filmes selecionada para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="57e68-112">Movies rating selected for United States.</span></span> <span data-ttu-id="57e68-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="57e68-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="57e68-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="57e68-114">tvRating</span></span>|[<span data-ttu-id="57e68-115">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="57e68-115">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="57e68-116">Classificação de TV selecionada para Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="57e68-116">TV rating selected for United States.</span></span> <span data-ttu-id="57e68-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="57e68-117">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57e68-118">Relações</span><span class="sxs-lookup"><span data-stu-id="57e68-118">Relationships</span></span>
<span data-ttu-id="57e68-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="57e68-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57e68-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="57e68-120">JSON Representation</span></span>
<span data-ttu-id="57e68-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="57e68-121">Here is a JSON representation of the resource.</span></span>
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



