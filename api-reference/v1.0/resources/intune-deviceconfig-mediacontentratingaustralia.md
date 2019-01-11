---
title: Tipo de recurso mediaContentRatingAustralia
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0860a17671b2923c2be9b5b469f93d443e808f53
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891480"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="a08ee-103">Tipo de recurso mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="a08ee-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="a08ee-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a08ee-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a08ee-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a08ee-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="a08ee-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a08ee-106">Properties</span></span>
|<span data-ttu-id="a08ee-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a08ee-107">Property</span></span>|<span data-ttu-id="a08ee-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a08ee-108">Type</span></span>|<span data-ttu-id="a08ee-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a08ee-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a08ee-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="a08ee-110">movieRating</span></span>|[<span data-ttu-id="a08ee-111">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="a08ee-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="a08ee-112">Filmes selecionado para Austrália de classificação.</span><span class="sxs-lookup"><span data-stu-id="a08ee-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="a08ee-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="a08ee-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="a08ee-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="a08ee-114">tvRating</span></span>|[<span data-ttu-id="a08ee-115">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="a08ee-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="a08ee-116">Classificação de TV selecionada para Austrália.</span><span class="sxs-lookup"><span data-stu-id="a08ee-116">TV rating selected for Australia.</span></span> <span data-ttu-id="a08ee-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="a08ee-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a08ee-118">Relações</span><span class="sxs-lookup"><span data-stu-id="a08ee-118">Relationships</span></span>
<span data-ttu-id="a08ee-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a08ee-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a08ee-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a08ee-120">JSON Representation</span></span>
<span data-ttu-id="a08ee-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a08ee-121">Here is a JSON representation of the resource.</span></span>
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



