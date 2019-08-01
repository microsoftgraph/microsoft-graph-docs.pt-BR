---
title: Tipo de recurso mediaContentRatingJapan
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8c4e4268857f2d76e1dcf01e047a492f80492a89
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031385"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="35c7f-103">Tipo de recurso mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="35c7f-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="35c7f-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="35c7f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35c7f-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="35c7f-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="35c7f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="35c7f-106">Properties</span></span>
|<span data-ttu-id="35c7f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35c7f-107">Property</span></span>|<span data-ttu-id="35c7f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="35c7f-108">Type</span></span>|<span data-ttu-id="35c7f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="35c7f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35c7f-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="35c7f-110">movieRating</span></span>|[<span data-ttu-id="35c7f-111">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="35c7f-111">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="35c7f-112">Classificação de filmes selecionada para o Japão.</span><span class="sxs-lookup"><span data-stu-id="35c7f-112">Movies rating selected for Japan.</span></span> <span data-ttu-id="35c7f-113">Os possíveis valores são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="35c7f-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="35c7f-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="35c7f-114">tvRating</span></span>|[<span data-ttu-id="35c7f-115">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="35c7f-115">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="35c7f-116">Classificação de TV selecionada para o Japão.</span><span class="sxs-lookup"><span data-stu-id="35c7f-116">TV rating selected for Japan.</span></span> <span data-ttu-id="35c7f-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="35c7f-117">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35c7f-118">Relações</span><span class="sxs-lookup"><span data-stu-id="35c7f-118">Relationships</span></span>
<span data-ttu-id="35c7f-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="35c7f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35c7f-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="35c7f-120">JSON Representation</span></span>
<span data-ttu-id="35c7f-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="35c7f-121">Here is a JSON representation of the resource.</span></span>
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



