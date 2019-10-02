---
title: Tipo de recurso mediaContentRatingJapan
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 398192d54c2e377d6d6a4cfad2e519b78d84420d
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359961"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="8c272-103">Tipo de recurso mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="8c272-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="8c272-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8c272-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c272-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8c272-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="8c272-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8c272-106">Properties</span></span>
|<span data-ttu-id="8c272-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c272-107">Property</span></span>|<span data-ttu-id="8c272-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c272-108">Type</span></span>|<span data-ttu-id="8c272-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c272-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c272-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="8c272-110">movieRating</span></span>|[<span data-ttu-id="8c272-111">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="8c272-111">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="8c272-112">Classificação de filmes selecionada para o Japão.</span><span class="sxs-lookup"><span data-stu-id="8c272-112">Movies rating selected for Japan.</span></span> <span data-ttu-id="8c272-113">Os possíveis valores são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="8c272-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="8c272-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="8c272-114">tvRating</span></span>|[<span data-ttu-id="8c272-115">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="8c272-115">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="8c272-116">Classificação de TV selecionada para o Japão.</span><span class="sxs-lookup"><span data-stu-id="8c272-116">TV rating selected for Japan.</span></span> <span data-ttu-id="8c272-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="8c272-117">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c272-118">Relações</span><span class="sxs-lookup"><span data-stu-id="8c272-118">Relationships</span></span>
<span data-ttu-id="8c272-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8c272-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c272-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8c272-120">JSON Representation</span></span>
<span data-ttu-id="8c272-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8c272-121">Here is a JSON representation of the resource.</span></span>
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




