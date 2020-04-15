---
title: Tipo de recurso mediaContentRatingAustralia
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b25b309e011645c376a23c08b8673a7579ae69ad
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43410131"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="a0bb9-103">Tipo de recurso mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="a0bb9-103">mediaContentRatingAustralia resource type</span></span>

<span data-ttu-id="a0bb9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0bb9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a0bb9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a0bb9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0bb9-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="a0bb9-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="a0bb9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0bb9-107">Properties</span></span>
|<span data-ttu-id="a0bb9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0bb9-108">Property</span></span>|<span data-ttu-id="a0bb9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0bb9-109">Type</span></span>|<span data-ttu-id="a0bb9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0bb9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0bb9-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="a0bb9-111">movieRating</span></span>|[<span data-ttu-id="a0bb9-112">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="a0bb9-112">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="a0bb9-113">Classificação de filmes selecionada para a Austrália.</span><span class="sxs-lookup"><span data-stu-id="a0bb9-113">Movies rating selected for Australia.</span></span> <span data-ttu-id="a0bb9-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="a0bb9-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="a0bb9-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="a0bb9-115">tvRating</span></span>|[<span data-ttu-id="a0bb9-116">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="a0bb9-116">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="a0bb9-117">Classificação de TV selecionada para a Austrália.</span><span class="sxs-lookup"><span data-stu-id="a0bb9-117">TV rating selected for Australia.</span></span> <span data-ttu-id="a0bb9-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="a0bb9-118">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0bb9-119">Relações</span><span class="sxs-lookup"><span data-stu-id="a0bb9-119">Relationships</span></span>
<span data-ttu-id="a0bb9-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a0bb9-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0bb9-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0bb9-121">JSON Representation</span></span>
<span data-ttu-id="a0bb9-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a0bb9-122">Here is a JSON representation of the resource.</span></span>
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







