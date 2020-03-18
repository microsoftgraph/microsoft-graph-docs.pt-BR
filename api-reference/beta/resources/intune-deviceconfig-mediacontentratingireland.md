---
title: Tipo de recurso mediaContentRatingIreland
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5b6e6dc939672d855b2fd25b47a54ea3f62d4280
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788573"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="8f765-103">Tipo de recurso mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="8f765-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="8f765-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8f765-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f765-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8f765-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f765-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8f765-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8f765-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8f765-107">Properties</span></span>
|<span data-ttu-id="8f765-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8f765-108">Property</span></span>|<span data-ttu-id="8f765-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f765-109">Type</span></span>|<span data-ttu-id="8f765-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f765-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f765-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="8f765-111">movieRating</span></span>|[<span data-ttu-id="8f765-112">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="8f765-112">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="8f765-113">Classificação de filmes selecionada para a Irlanda.</span><span class="sxs-lookup"><span data-stu-id="8f765-113">Movies rating selected for Ireland.</span></span> <span data-ttu-id="8f765-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="8f765-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="8f765-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="8f765-115">tvRating</span></span>|[<span data-ttu-id="8f765-116">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="8f765-116">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="8f765-117">Classificação de TV selecionada para a Irlanda.</span><span class="sxs-lookup"><span data-stu-id="8f765-117">TV rating selected for Ireland.</span></span> <span data-ttu-id="8f765-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="8f765-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f765-119">Relações</span><span class="sxs-lookup"><span data-stu-id="8f765-119">Relationships</span></span>
<span data-ttu-id="8f765-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8f765-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8f765-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8f765-121">JSON Representation</span></span>
<span data-ttu-id="8f765-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8f765-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```



