---
title: Tipo de recurso mediaContentRatingJapan
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 691b723f2140bbdda370bbf5b46330579ca0a871
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758831"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="76266-103">Tipo de recurso mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="76266-103">mediaContentRatingJapan resource type</span></span>

<span data-ttu-id="76266-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76266-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76266-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="76266-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76266-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="76266-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="76266-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="76266-107">Properties</span></span>
|<span data-ttu-id="76266-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76266-108">Property</span></span>|<span data-ttu-id="76266-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="76266-109">Type</span></span>|<span data-ttu-id="76266-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="76266-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76266-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="76266-111">movieRating</span></span>|[<span data-ttu-id="76266-112">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="76266-112">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="76266-113">Classificação de filmes selecionada para o Japão.</span><span class="sxs-lookup"><span data-stu-id="76266-113">Movies rating selected for Japan.</span></span> <span data-ttu-id="76266-114">Os possíveis valores são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="76266-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="76266-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="76266-115">tvRating</span></span>|[<span data-ttu-id="76266-116">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="76266-116">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="76266-117">Classificação de TV selecionada para o Japão.</span><span class="sxs-lookup"><span data-stu-id="76266-117">TV rating selected for Japan.</span></span> <span data-ttu-id="76266-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="76266-118">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="76266-119">Relações</span><span class="sxs-lookup"><span data-stu-id="76266-119">Relationships</span></span>
<span data-ttu-id="76266-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="76266-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="76266-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="76266-121">JSON Representation</span></span>
<span data-ttu-id="76266-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="76266-122">Here is a JSON representation of the resource.</span></span>
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




