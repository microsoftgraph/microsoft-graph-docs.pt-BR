---
title: Tipo de recurso mediaContentRatingAustralia
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5f3f12cc233c1accfad05ccec92d412c75426d1a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27952843"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="00fde-103">Tipo de recurso mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="00fde-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="00fde-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="00fde-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00fde-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="00fde-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="00fde-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="00fde-106">Properties</span></span>
|<span data-ttu-id="00fde-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="00fde-107">Property</span></span>|<span data-ttu-id="00fde-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="00fde-108">Type</span></span>|<span data-ttu-id="00fde-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="00fde-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00fde-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="00fde-110">movieRating</span></span>|[<span data-ttu-id="00fde-111">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="00fde-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="00fde-112">Filmes selecionado para Austrália de classificação.</span><span class="sxs-lookup"><span data-stu-id="00fde-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="00fde-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="00fde-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="00fde-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="00fde-114">tvRating</span></span>|[<span data-ttu-id="00fde-115">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="00fde-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="00fde-116">Classificação de TV selecionada para Austrália.</span><span class="sxs-lookup"><span data-stu-id="00fde-116">TV rating selected for Australia.</span></span> <span data-ttu-id="00fde-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="00fde-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00fde-118">Relações</span><span class="sxs-lookup"><span data-stu-id="00fde-118">Relationships</span></span>
<span data-ttu-id="00fde-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="00fde-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="00fde-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="00fde-120">JSON Representation</span></span>
<span data-ttu-id="00fde-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="00fde-121">Here is a JSON representation of the resource.</span></span>
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



