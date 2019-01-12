---
title: Tipo de recurso mediaContentRatingUnitedKingdom
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8bdcd67bbc81cb5436c6be22c395a6c9804b0637
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951590"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="9ef3d-103">Tipo de recurso mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="9ef3d-103">mediaContentRatingUnitedKingdom resource type</span></span>

> <span data-ttu-id="9ef3d-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9ef3d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ef3d-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9ef3d-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="9ef3d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9ef3d-106">Properties</span></span>
|<span data-ttu-id="9ef3d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ef3d-107">Property</span></span>|<span data-ttu-id="9ef3d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ef3d-108">Type</span></span>|<span data-ttu-id="9ef3d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ef3d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ef3d-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="9ef3d-110">movieRating</span></span>|[<span data-ttu-id="9ef3d-111">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="9ef3d-111">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="9ef3d-112">Filmes classificação selecionado para o Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="9ef3d-112">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="9ef3d-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="9ef3d-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="9ef3d-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="9ef3d-114">tvRating</span></span>|[<span data-ttu-id="9ef3d-115">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="9ef3d-115">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="9ef3d-116">Classificação de TV selecionada para o Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="9ef3d-116">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="9ef3d-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="9ef3d-117">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ef3d-118">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="9ef3d-118">Relationships</span></span>
<span data-ttu-id="9ef3d-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9ef3d-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9ef3d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ef3d-120">JSON Representation</span></span>
<span data-ttu-id="9ef3d-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9ef3d-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```



