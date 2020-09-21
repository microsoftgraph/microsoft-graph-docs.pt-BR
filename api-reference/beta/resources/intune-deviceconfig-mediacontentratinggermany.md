---
title: Tipo de recurso mediaContentRatingGermany
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 568f88dd3d595e3fafdf1ac8d201752d19235a8d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47968427"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="c741d-103">Tipo de recurso mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="c741d-103">mediaContentRatingGermany resource type</span></span>

<span data-ttu-id="c741d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c741d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c741d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c741d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c741d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c741d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c741d-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c741d-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c741d-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c741d-108">Properties</span></span>
|<span data-ttu-id="c741d-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c741d-109">Property</span></span>|<span data-ttu-id="c741d-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c741d-110">Type</span></span>|<span data-ttu-id="c741d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c741d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c741d-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="c741d-112">movieRating</span></span>|[<span data-ttu-id="c741d-113">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="c741d-113">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="c741d-114">Classificação de filmes selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="c741d-114">Movies rating selected for Germany.</span></span> <span data-ttu-id="c741d-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="c741d-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="c741d-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="c741d-116">tvRating</span></span>|[<span data-ttu-id="c741d-117">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c741d-117">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="c741d-118">Classificação de TV selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="c741d-118">TV rating selected for Germany.</span></span> <span data-ttu-id="c741d-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="c741d-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c741d-120">Relações</span><span class="sxs-lookup"><span data-stu-id="c741d-120">Relationships</span></span>
<span data-ttu-id="c741d-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c741d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c741d-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c741d-122">JSON Representation</span></span>
<span data-ttu-id="c741d-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c741d-123">Here is a JSON representation of the resource.</span></span>
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






