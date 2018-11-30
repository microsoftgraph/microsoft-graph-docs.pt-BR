---
title: Tipo de recurso mediaContentRatingUnitedStates
description: Ainda não documentado
ms.openlocfilehash: b96241f31e232f39f62a09d7fff8560e5a89e237
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006424"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="434a1-103">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="434a1-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="434a1-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="434a1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="434a1-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="434a1-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="434a1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="434a1-106">Properties</span></span>
|<span data-ttu-id="434a1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="434a1-107">Property</span></span>|<span data-ttu-id="434a1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="434a1-108">Type</span></span>|<span data-ttu-id="434a1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="434a1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="434a1-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="434a1-110">movieRating</span></span>|[<span data-ttu-id="434a1-111">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="434a1-111">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="434a1-112">Filmes classificação selecionado para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="434a1-112">Movies rating selected for United States.</span></span> <span data-ttu-id="434a1-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="434a1-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="434a1-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="434a1-114">tvRating</span></span>|[<span data-ttu-id="434a1-115">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="434a1-115">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="434a1-116">Classificação de TV selecionada para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="434a1-116">TV rating selected for United States.</span></span> <span data-ttu-id="434a1-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="434a1-117">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="434a1-118">Relações</span><span class="sxs-lookup"><span data-stu-id="434a1-118">Relationships</span></span>
<span data-ttu-id="434a1-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="434a1-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="434a1-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="434a1-120">JSON Representation</span></span>
<span data-ttu-id="434a1-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="434a1-121">Here is a JSON representation of the resource.</span></span>
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



