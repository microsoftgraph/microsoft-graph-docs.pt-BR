---
title: Tipo de recurso mediaContentRatingAustralia
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: af27f6f4cfc49e90186aed4ed266b62c9b1a0343
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788601"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="c8124-103">Tipo de recurso mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="c8124-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="c8124-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c8124-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8124-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c8124-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8124-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c8124-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c8124-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c8124-107">Properties</span></span>
|<span data-ttu-id="c8124-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8124-108">Property</span></span>|<span data-ttu-id="c8124-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8124-109">Type</span></span>|<span data-ttu-id="c8124-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8124-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8124-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="c8124-111">movieRating</span></span>|[<span data-ttu-id="c8124-112">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="c8124-112">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="c8124-113">Classificação de filmes selecionada para a Austrália.</span><span class="sxs-lookup"><span data-stu-id="c8124-113">Movies rating selected for Australia.</span></span> <span data-ttu-id="c8124-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="c8124-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="c8124-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="c8124-115">tvRating</span></span>|[<span data-ttu-id="c8124-116">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c8124-116">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="c8124-117">Classificação de TV selecionada para a Austrália.</span><span class="sxs-lookup"><span data-stu-id="c8124-117">TV rating selected for Australia.</span></span> <span data-ttu-id="c8124-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="c8124-118">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8124-119">Relações</span><span class="sxs-lookup"><span data-stu-id="c8124-119">Relationships</span></span>
<span data-ttu-id="c8124-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c8124-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8124-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c8124-121">JSON Representation</span></span>
<span data-ttu-id="c8124-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c8124-122">Here is a JSON representation of the resource.</span></span>
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



