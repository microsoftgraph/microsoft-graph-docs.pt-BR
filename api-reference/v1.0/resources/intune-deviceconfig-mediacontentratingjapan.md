---
title: Tipo de recurso mediaContentRatingJapan
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: baa36c189e84e7671a9b9387bc0737dd4076bf75
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003098"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="96f74-103">Tipo de recurso mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="96f74-103">mediaContentRatingJapan resource type</span></span>

<span data-ttu-id="96f74-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96f74-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96f74-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="96f74-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96f74-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="96f74-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="96f74-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="96f74-107">Properties</span></span>
|<span data-ttu-id="96f74-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96f74-108">Property</span></span>|<span data-ttu-id="96f74-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="96f74-109">Type</span></span>|<span data-ttu-id="96f74-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="96f74-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96f74-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="96f74-111">movieRating</span></span>|[<span data-ttu-id="96f74-112">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="96f74-112">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="96f74-113">Classificação de filmes selecionada para o Japão.</span><span class="sxs-lookup"><span data-stu-id="96f74-113">Movies rating selected for Japan.</span></span> <span data-ttu-id="96f74-114">Os possíveis valores são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="96f74-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="96f74-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="96f74-115">tvRating</span></span>|[<span data-ttu-id="96f74-116">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="96f74-116">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="96f74-117">Classificação de TV selecionada para o Japão.</span><span class="sxs-lookup"><span data-stu-id="96f74-117">TV rating selected for Japan.</span></span> <span data-ttu-id="96f74-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="96f74-118">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96f74-119">Relações</span><span class="sxs-lookup"><span data-stu-id="96f74-119">Relationships</span></span>
<span data-ttu-id="96f74-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96f74-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="96f74-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="96f74-121">JSON Representation</span></span>
<span data-ttu-id="96f74-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="96f74-122">Here is a JSON representation of the resource.</span></span>
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









