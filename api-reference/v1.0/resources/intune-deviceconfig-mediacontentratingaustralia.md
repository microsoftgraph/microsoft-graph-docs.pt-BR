---
title: Tipo de recurso mediaContentRatingAustralia
description: Ainda não documentado
ms.openlocfilehash: f60df6c4948d0e0208b545a8a25e31ca29247879
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005237"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="b7f4d-103">Tipo de recurso mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="b7f4d-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="b7f4d-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b7f4d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b7f4d-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b7f4d-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="b7f4d-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b7f4d-106">Properties</span></span>
|<span data-ttu-id="b7f4d-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b7f4d-107">Property</span></span>|<span data-ttu-id="b7f4d-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b7f4d-108">Type</span></span>|<span data-ttu-id="b7f4d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b7f4d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7f4d-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="b7f4d-110">movieRating</span></span>|[<span data-ttu-id="b7f4d-111">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="b7f4d-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="b7f4d-112">Filmes selecionado para Austrália de classificação.</span><span class="sxs-lookup"><span data-stu-id="b7f4d-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="b7f4d-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="b7f4d-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="b7f4d-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="b7f4d-114">tvRating</span></span>|[<span data-ttu-id="b7f4d-115">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="b7f4d-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="b7f4d-116">Classificação de TV selecionada para Austrália.</span><span class="sxs-lookup"><span data-stu-id="b7f4d-116">TV rating selected for Australia.</span></span> <span data-ttu-id="b7f4d-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="b7f4d-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7f4d-118">Relações</span><span class="sxs-lookup"><span data-stu-id="b7f4d-118">Relationships</span></span>
<span data-ttu-id="b7f4d-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b7f4d-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b7f4d-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b7f4d-120">JSON Representation</span></span>
<span data-ttu-id="b7f4d-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b7f4d-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```



