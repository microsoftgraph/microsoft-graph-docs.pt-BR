---
title: Tipo de recurso mediaContentRatingGermany
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 550e444d6acf3bea53f4d1c68a3a09da5a16dfcd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003133"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="3cd4d-103">Tipo de recurso mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="3cd4d-103">mediaContentRatingGermany resource type</span></span>

<span data-ttu-id="3cd4d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cd4d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3cd4d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3cd4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cd4d-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3cd4d-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="3cd4d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3cd4d-107">Properties</span></span>
|<span data-ttu-id="3cd4d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3cd4d-108">Property</span></span>|<span data-ttu-id="3cd4d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3cd4d-109">Type</span></span>|<span data-ttu-id="3cd4d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3cd4d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cd4d-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="3cd4d-111">movieRating</span></span>|[<span data-ttu-id="3cd4d-112">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="3cd4d-112">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="3cd4d-113">Classificação de filmes selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="3cd4d-113">Movies rating selected for Germany.</span></span> <span data-ttu-id="3cd4d-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="3cd4d-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="3cd4d-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="3cd4d-115">tvRating</span></span>|[<span data-ttu-id="3cd4d-116">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="3cd4d-116">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="3cd4d-117">Classificação de TV selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="3cd4d-117">TV rating selected for Germany.</span></span> <span data-ttu-id="3cd4d-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="3cd4d-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3cd4d-119">Relações</span><span class="sxs-lookup"><span data-stu-id="3cd4d-119">Relationships</span></span>
<span data-ttu-id="3cd4d-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3cd4d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3cd4d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3cd4d-121">JSON Representation</span></span>
<span data-ttu-id="3cd4d-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3cd4d-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```









