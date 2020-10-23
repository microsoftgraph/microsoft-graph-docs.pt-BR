---
title: Tipo de recurso mediaContentRatingIreland
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 53ae5d7686bd8f9820c227441b34d898d4a9db4e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692461"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="78fac-103">Tipo de recurso mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="78fac-103">mediaContentRatingIreland resource type</span></span>

<span data-ttu-id="78fac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78fac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78fac-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="78fac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78fac-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="78fac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78fac-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="78fac-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="78fac-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="78fac-108">Properties</span></span>
|<span data-ttu-id="78fac-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78fac-109">Property</span></span>|<span data-ttu-id="78fac-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="78fac-110">Type</span></span>|<span data-ttu-id="78fac-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="78fac-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78fac-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="78fac-112">movieRating</span></span>|[<span data-ttu-id="78fac-113">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="78fac-113">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="78fac-114">Classificação de filmes selecionada para a Irlanda.</span><span class="sxs-lookup"><span data-stu-id="78fac-114">Movies rating selected for Ireland.</span></span> <span data-ttu-id="78fac-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="78fac-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="78fac-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="78fac-116">tvRating</span></span>|[<span data-ttu-id="78fac-117">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="78fac-117">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="78fac-118">Classificação de TV selecionada para a Irlanda.</span><span class="sxs-lookup"><span data-stu-id="78fac-118">TV rating selected for Ireland.</span></span> <span data-ttu-id="78fac-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="78fac-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78fac-120">Relações</span><span class="sxs-lookup"><span data-stu-id="78fac-120">Relationships</span></span>
<span data-ttu-id="78fac-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="78fac-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="78fac-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="78fac-122">JSON Representation</span></span>
<span data-ttu-id="78fac-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="78fac-123">Here is a JSON representation of the resource.</span></span>
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





