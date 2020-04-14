---
title: Tipo de recurso mediaContentRatingGermany
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e146adc4b2d2e550701a6f152efcdefb41758644
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437212"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="086ff-103">Tipo de recurso mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="086ff-103">mediaContentRatingGermany resource type</span></span>

<span data-ttu-id="086ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="086ff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="086ff-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="086ff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="086ff-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="086ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="086ff-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="086ff-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="086ff-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="086ff-108">Properties</span></span>
|<span data-ttu-id="086ff-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="086ff-109">Property</span></span>|<span data-ttu-id="086ff-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="086ff-110">Type</span></span>|<span data-ttu-id="086ff-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="086ff-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="086ff-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="086ff-112">movieRating</span></span>|[<span data-ttu-id="086ff-113">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="086ff-113">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="086ff-114">Classificação de filmes selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="086ff-114">Movies rating selected for Germany.</span></span> <span data-ttu-id="086ff-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="086ff-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="086ff-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="086ff-116">tvRating</span></span>|[<span data-ttu-id="086ff-117">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="086ff-117">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="086ff-118">Classificação de TV selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="086ff-118">TV rating selected for Germany.</span></span> <span data-ttu-id="086ff-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="086ff-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="086ff-120">Relações</span><span class="sxs-lookup"><span data-stu-id="086ff-120">Relationships</span></span>
<span data-ttu-id="086ff-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="086ff-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="086ff-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="086ff-122">JSON Representation</span></span>
<span data-ttu-id="086ff-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="086ff-123">Here is a JSON representation of the resource.</span></span>
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



