---
title: Tipo de recurso mediaContentRatingJapan
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 703e34fa55f33c3ce6fd72ec196f314ffd77f057
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368706"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="1a212-103">Tipo de recurso mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="1a212-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="1a212-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1a212-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a212-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1a212-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a212-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1a212-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1a212-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1a212-107">Properties</span></span>
|<span data-ttu-id="1a212-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1a212-108">Property</span></span>|<span data-ttu-id="1a212-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1a212-109">Type</span></span>|<span data-ttu-id="1a212-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a212-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a212-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="1a212-111">movieRating</span></span>|[<span data-ttu-id="1a212-112">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="1a212-112">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="1a212-113">Classificação de filmes selecionada para o Japão.</span><span class="sxs-lookup"><span data-stu-id="1a212-113">Movies rating selected for Japan.</span></span> <span data-ttu-id="1a212-114">Os possíveis valores são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="1a212-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="1a212-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="1a212-115">tvRating</span></span>|[<span data-ttu-id="1a212-116">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="1a212-116">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="1a212-117">Classificação de TV selecionada para o Japão.</span><span class="sxs-lookup"><span data-stu-id="1a212-117">TV rating selected for Japan.</span></span> <span data-ttu-id="1a212-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="1a212-118">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a212-119">Relações</span><span class="sxs-lookup"><span data-stu-id="1a212-119">Relationships</span></span>
<span data-ttu-id="1a212-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1a212-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a212-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1a212-121">JSON Representation</span></span>
<span data-ttu-id="1a212-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1a212-122">Here is a JSON representation of the resource.</span></span>
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



