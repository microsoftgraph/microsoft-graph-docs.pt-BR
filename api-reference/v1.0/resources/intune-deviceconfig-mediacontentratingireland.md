---
title: Tipo de recurso mediaContentRatingIreland
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 531768883b88e8fc89fe00c1df7a8a9e8767a408
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934874"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="a148d-103">Tipo de recurso mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="a148d-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="a148d-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a148d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a148d-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a148d-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="a148d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a148d-106">Properties</span></span>
|<span data-ttu-id="a148d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a148d-107">Property</span></span>|<span data-ttu-id="a148d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a148d-108">Type</span></span>|<span data-ttu-id="a148d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a148d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a148d-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="a148d-110">movieRating</span></span>|[<span data-ttu-id="a148d-111">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="a148d-111">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="a148d-112">Filmes selecionado para Irlanda de classificação.</span><span class="sxs-lookup"><span data-stu-id="a148d-112">Movies rating selected for Ireland.</span></span> <span data-ttu-id="a148d-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="a148d-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="a148d-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="a148d-114">tvRating</span></span>|[<span data-ttu-id="a148d-115">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="a148d-115">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="a148d-116">Classificação de TV selecionada para Irlanda.</span><span class="sxs-lookup"><span data-stu-id="a148d-116">TV rating selected for Ireland.</span></span> <span data-ttu-id="a148d-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="a148d-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a148d-118">Relações</span><span class="sxs-lookup"><span data-stu-id="a148d-118">Relationships</span></span>
<span data-ttu-id="a148d-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a148d-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a148d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a148d-120">JSON Representation</span></span>
<span data-ttu-id="a148d-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a148d-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```



