---
title: Tipo de recurso mediaContentRatingAustralia
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f2d3c6808b6fa350ea1ca5965eb7c123c0e70287
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368790"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="b1d1d-103">Tipo de recurso mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="b1d1d-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="b1d1d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b1d1d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1d1d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b1d1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1d1d-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b1d1d-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b1d1d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b1d1d-107">Properties</span></span>
|<span data-ttu-id="b1d1d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b1d1d-108">Property</span></span>|<span data-ttu-id="b1d1d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1d1d-109">Type</span></span>|<span data-ttu-id="b1d1d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1d1d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1d1d-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="b1d1d-111">movieRating</span></span>|[<span data-ttu-id="b1d1d-112">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="b1d1d-112">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="b1d1d-113">Classificação de filmes selecionada para a Austrália.</span><span class="sxs-lookup"><span data-stu-id="b1d1d-113">Movies rating selected for Australia.</span></span> <span data-ttu-id="b1d1d-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="b1d1d-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="b1d1d-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="b1d1d-115">tvRating</span></span>|[<span data-ttu-id="b1d1d-116">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="b1d1d-116">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="b1d1d-117">Classificação de TV selecionada para a Austrália.</span><span class="sxs-lookup"><span data-stu-id="b1d1d-117">TV rating selected for Australia.</span></span> <span data-ttu-id="b1d1d-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="b1d1d-118">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1d1d-119">Relações</span><span class="sxs-lookup"><span data-stu-id="b1d1d-119">Relationships</span></span>
<span data-ttu-id="b1d1d-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b1d1d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1d1d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b1d1d-121">JSON Representation</span></span>
<span data-ttu-id="b1d1d-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b1d1d-122">Here is a JSON representation of the resource.</span></span>
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



