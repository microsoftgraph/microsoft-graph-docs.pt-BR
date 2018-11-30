---
title: Tipo de recurso mediaContentRatingIreland
description: Ainda não documentado
ms.openlocfilehash: b4348e6f73730d59e6e67b3e102b9ad9caa98add
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003756"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="3d47b-103">Tipo de recurso mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="3d47b-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="3d47b-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="3d47b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3d47b-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3d47b-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="3d47b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3d47b-106">Properties</span></span>
|<span data-ttu-id="3d47b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3d47b-107">Property</span></span>|<span data-ttu-id="3d47b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="3d47b-108">Type</span></span>|<span data-ttu-id="3d47b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="3d47b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d47b-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="3d47b-110">movieRating</span></span>|[<span data-ttu-id="3d47b-111">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="3d47b-111">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="3d47b-112">Filmes selecionado para Irlanda de classificação.</span><span class="sxs-lookup"><span data-stu-id="3d47b-112">Movies rating selected for Ireland.</span></span> <span data-ttu-id="3d47b-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="3d47b-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="3d47b-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="3d47b-114">tvRating</span></span>|[<span data-ttu-id="3d47b-115">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="3d47b-115">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="3d47b-116">Classificação de TV selecionada para Irlanda.</span><span class="sxs-lookup"><span data-stu-id="3d47b-116">TV rating selected for Ireland.</span></span> <span data-ttu-id="3d47b-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="3d47b-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3d47b-118">Relações</span><span class="sxs-lookup"><span data-stu-id="3d47b-118">Relationships</span></span>
<span data-ttu-id="3d47b-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3d47b-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3d47b-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3d47b-120">JSON Representation</span></span>
<span data-ttu-id="3d47b-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3d47b-121">Here is a JSON representation of the resource.</span></span>
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



