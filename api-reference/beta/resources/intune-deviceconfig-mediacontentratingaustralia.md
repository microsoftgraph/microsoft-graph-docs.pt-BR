---
title: Tipo de recurso mediaContentRatingAustralia
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4c5cba0b06d00605510003a71aa826e11ae79426
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000869"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="6daf4-103">Tipo de recurso mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="6daf4-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="6daf4-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6daf4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6daf4-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6daf4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6daf4-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6daf4-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6daf4-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6daf4-107">Properties</span></span>
|<span data-ttu-id="6daf4-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6daf4-108">Property</span></span>|<span data-ttu-id="6daf4-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6daf4-109">Type</span></span>|<span data-ttu-id="6daf4-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6daf4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6daf4-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="6daf4-111">movieRating</span></span>|[<span data-ttu-id="6daf4-112">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="6daf4-112">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="6daf4-113">Classificação de filmes selecionada para a Austrália.</span><span class="sxs-lookup"><span data-stu-id="6daf4-113">Movies rating selected for Australia.</span></span> <span data-ttu-id="6daf4-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="6daf4-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="6daf4-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="6daf4-115">tvRating</span></span>|[<span data-ttu-id="6daf4-116">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="6daf4-116">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="6daf4-117">Classificação de TV selecionada para a Austrália.</span><span class="sxs-lookup"><span data-stu-id="6daf4-117">TV rating selected for Australia.</span></span> <span data-ttu-id="6daf4-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="6daf4-118">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6daf4-119">Relações</span><span class="sxs-lookup"><span data-stu-id="6daf4-119">Relationships</span></span>
<span data-ttu-id="6daf4-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6daf4-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6daf4-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6daf4-121">JSON Representation</span></span>
<span data-ttu-id="6daf4-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6daf4-122">Here is a JSON representation of the resource.</span></span>
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





