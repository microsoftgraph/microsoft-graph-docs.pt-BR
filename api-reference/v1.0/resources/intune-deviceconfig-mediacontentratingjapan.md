---
title: Tipo de recurso mediaContentRatingJapan
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0543aec86312d90a5896ed3f06f004c87d8e6a58
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250303"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="ccb92-103">Tipo de recurso mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="ccb92-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="ccb92-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ccb92-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccb92-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ccb92-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ccb92-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ccb92-106">Properties</span></span>
|<span data-ttu-id="ccb92-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ccb92-107">Property</span></span>|<span data-ttu-id="ccb92-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ccb92-108">Type</span></span>|<span data-ttu-id="ccb92-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ccb92-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccb92-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="ccb92-110">movieRating</span></span>|[<span data-ttu-id="ccb92-111">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="ccb92-111">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="ccb92-112">Classificação de filmes selecionada para o Japão.</span><span class="sxs-lookup"><span data-stu-id="ccb92-112">Movies rating selected for Japan.</span></span> <span data-ttu-id="ccb92-113">Os possíveis valores são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="ccb92-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="ccb92-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="ccb92-114">tvRating</span></span>|[<span data-ttu-id="ccb92-115">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="ccb92-115">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="ccb92-116">Classificação de TV selecionada para o Japão.</span><span class="sxs-lookup"><span data-stu-id="ccb92-116">TV rating selected for Japan.</span></span> <span data-ttu-id="ccb92-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="ccb92-117">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ccb92-118">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="ccb92-118">Relationships</span></span>
<span data-ttu-id="ccb92-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ccb92-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ccb92-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ccb92-120">JSON Representation</span></span>
<span data-ttu-id="ccb92-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ccb92-121">Here is a JSON representation of the resource.</span></span>
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



