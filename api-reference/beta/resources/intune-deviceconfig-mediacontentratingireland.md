---
title: Tipo de recurso mediaContentRatingIreland
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f497922920ab6826bf11ad0ed78234d2c180f7a7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000800"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="01614-103">Tipo de recurso mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="01614-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="01614-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="01614-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01614-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="01614-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01614-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="01614-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="01614-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="01614-107">Properties</span></span>
|<span data-ttu-id="01614-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01614-108">Property</span></span>|<span data-ttu-id="01614-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="01614-109">Type</span></span>|<span data-ttu-id="01614-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="01614-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01614-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="01614-111">movieRating</span></span>|[<span data-ttu-id="01614-112">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="01614-112">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="01614-113">Classificação de filmes selecionada para a Irlanda.</span><span class="sxs-lookup"><span data-stu-id="01614-113">Movies rating selected for Ireland.</span></span> <span data-ttu-id="01614-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="01614-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="01614-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="01614-115">tvRating</span></span>|[<span data-ttu-id="01614-116">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="01614-116">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="01614-117">Classificação de TV selecionada para a Irlanda.</span><span class="sxs-lookup"><span data-stu-id="01614-117">TV rating selected for Ireland.</span></span> <span data-ttu-id="01614-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="01614-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01614-119">Relações</span><span class="sxs-lookup"><span data-stu-id="01614-119">Relationships</span></span>
<span data-ttu-id="01614-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="01614-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="01614-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="01614-121">JSON Representation</span></span>
<span data-ttu-id="01614-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="01614-122">Here is a JSON representation of the resource.</span></span>
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





