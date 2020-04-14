---
title: Tipo de recurso mediaContentRatingJapan
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 52df25bb4a6a6e7615acb535741edfe70c122415
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437190"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="2f88a-103">Tipo de recurso mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="2f88a-103">mediaContentRatingJapan resource type</span></span>

<span data-ttu-id="2f88a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f88a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f88a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2f88a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f88a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2f88a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f88a-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2f88a-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="2f88a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2f88a-108">Properties</span></span>
|<span data-ttu-id="2f88a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2f88a-109">Property</span></span>|<span data-ttu-id="2f88a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2f88a-110">Type</span></span>|<span data-ttu-id="2f88a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f88a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f88a-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="2f88a-112">movieRating</span></span>|[<span data-ttu-id="2f88a-113">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="2f88a-113">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="2f88a-114">Classificação de filmes selecionada para o Japão.</span><span class="sxs-lookup"><span data-stu-id="2f88a-114">Movies rating selected for Japan.</span></span> <span data-ttu-id="2f88a-115">Os possíveis valores são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="2f88a-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="2f88a-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="2f88a-116">tvRating</span></span>|[<span data-ttu-id="2f88a-117">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="2f88a-117">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="2f88a-118">Classificação de TV selecionada para o Japão.</span><span class="sxs-lookup"><span data-stu-id="2f88a-118">TV rating selected for Japan.</span></span> <span data-ttu-id="2f88a-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="2f88a-119">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f88a-120">Relações</span><span class="sxs-lookup"><span data-stu-id="2f88a-120">Relationships</span></span>
<span data-ttu-id="2f88a-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2f88a-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f88a-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2f88a-122">JSON Representation</span></span>
<span data-ttu-id="2f88a-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2f88a-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```



