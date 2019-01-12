---
title: Tipo de recurso mediaContentRatingUnitedStates
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3e37a707b7ad190ddc1f3206f149d0dcc3c1aad3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27959220"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="d99f1-103">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="d99f1-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="d99f1-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d99f1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d99f1-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d99f1-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="d99f1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d99f1-106">Properties</span></span>
|<span data-ttu-id="d99f1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d99f1-107">Property</span></span>|<span data-ttu-id="d99f1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d99f1-108">Type</span></span>|<span data-ttu-id="d99f1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d99f1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d99f1-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="d99f1-110">movieRating</span></span>|[<span data-ttu-id="d99f1-111">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="d99f1-111">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="d99f1-112">Filmes classificação selecionado para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="d99f1-112">Movies rating selected for United States.</span></span> <span data-ttu-id="d99f1-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="d99f1-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="d99f1-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="d99f1-114">tvRating</span></span>|[<span data-ttu-id="d99f1-115">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="d99f1-115">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="d99f1-116">Classificação de TV selecionada para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="d99f1-116">TV rating selected for United States.</span></span> <span data-ttu-id="d99f1-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="d99f1-117">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d99f1-118">Relações</span><span class="sxs-lookup"><span data-stu-id="d99f1-118">Relationships</span></span>
<span data-ttu-id="d99f1-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d99f1-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d99f1-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d99f1-120">JSON Representation</span></span>
<span data-ttu-id="d99f1-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d99f1-121">Here is a JSON representation of the resource.</span></span>
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



