---
title: Tipo de recurso mediaContentRatingAustralia
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37e42c3629e73d8dc629ba754583f8023c168b30
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572371"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="670f0-103">Tipo de recurso mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="670f0-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="670f0-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="670f0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="670f0-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="670f0-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="670f0-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="670f0-106">Properties</span></span>
|<span data-ttu-id="670f0-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="670f0-107">Property</span></span>|<span data-ttu-id="670f0-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="670f0-108">Type</span></span>|<span data-ttu-id="670f0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="670f0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="670f0-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="670f0-110">movieRating</span></span>|[<span data-ttu-id="670f0-111">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="670f0-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="670f0-112">Classificação de filmes selecionada para a Austrália.</span><span class="sxs-lookup"><span data-stu-id="670f0-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="670f0-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="670f0-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="670f0-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="670f0-114">tvRating</span></span>|[<span data-ttu-id="670f0-115">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="670f0-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="670f0-116">Classificação de TV selecionada para a Austrália.</span><span class="sxs-lookup"><span data-stu-id="670f0-116">TV rating selected for Australia.</span></span> <span data-ttu-id="670f0-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="670f0-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="670f0-118">Relações</span><span class="sxs-lookup"><span data-stu-id="670f0-118">Relationships</span></span>
<span data-ttu-id="670f0-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="670f0-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="670f0-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="670f0-120">JSON Representation</span></span>
<span data-ttu-id="670f0-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="670f0-121">Here is a JSON representation of the resource.</span></span>
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



