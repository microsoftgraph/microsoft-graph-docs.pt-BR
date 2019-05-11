---
title: Tipo de recurso mediaContentRatingJapan
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8b1c79e68a530d176445b0395fdb7c4d50996485
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33950883"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="6c754-103">Tipo de recurso mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="6c754-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="6c754-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6c754-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c754-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6c754-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c754-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6c754-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6c754-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6c754-107">Properties</span></span>
|<span data-ttu-id="6c754-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c754-108">Property</span></span>|<span data-ttu-id="6c754-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c754-109">Type</span></span>|<span data-ttu-id="6c754-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c754-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c754-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="6c754-111">movieRating</span></span>|[<span data-ttu-id="6c754-112">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="6c754-112">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="6c754-113">Classificação de filmes selecionada para o Japão.</span><span class="sxs-lookup"><span data-stu-id="6c754-113">Movies rating selected for Japan.</span></span> <span data-ttu-id="6c754-114">Os possíveis valores são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="6c754-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="6c754-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="6c754-115">tvRating</span></span>|[<span data-ttu-id="6c754-116">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="6c754-116">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="6c754-117">Classificação de TV selecionada para o Japão.</span><span class="sxs-lookup"><span data-stu-id="6c754-117">TV rating selected for Japan.</span></span> <span data-ttu-id="6c754-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="6c754-118">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c754-119">Relações</span><span class="sxs-lookup"><span data-stu-id="6c754-119">Relationships</span></span>
<span data-ttu-id="6c754-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6c754-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c754-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6c754-121">JSON Representation</span></span>
<span data-ttu-id="6c754-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6c754-122">Here is a JSON representation of the resource.</span></span>
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




