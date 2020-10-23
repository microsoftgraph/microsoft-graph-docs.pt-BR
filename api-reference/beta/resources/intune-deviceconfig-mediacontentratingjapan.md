---
title: Tipo de recurso mediaContentRatingJapan
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 64f4a45d9fda194f18ccecc6a03102d2dfb24894
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707182"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="0cc47-103">Tipo de recurso mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="0cc47-103">mediaContentRatingJapan resource type</span></span>

<span data-ttu-id="0cc47-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0cc47-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0cc47-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0cc47-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cc47-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0cc47-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cc47-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0cc47-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="0cc47-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0cc47-108">Properties</span></span>
|<span data-ttu-id="0cc47-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0cc47-109">Property</span></span>|<span data-ttu-id="0cc47-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0cc47-110">Type</span></span>|<span data-ttu-id="0cc47-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cc47-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cc47-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="0cc47-112">movieRating</span></span>|[<span data-ttu-id="0cc47-113">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="0cc47-113">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="0cc47-114">Classificação de filmes selecionada para o Japão.</span><span class="sxs-lookup"><span data-stu-id="0cc47-114">Movies rating selected for Japan.</span></span> <span data-ttu-id="0cc47-115">Os possíveis valores são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="0cc47-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="0cc47-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="0cc47-116">tvRating</span></span>|[<span data-ttu-id="0cc47-117">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="0cc47-117">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="0cc47-118">Classificação de TV selecionada para o Japão.</span><span class="sxs-lookup"><span data-stu-id="0cc47-118">TV rating selected for Japan.</span></span> <span data-ttu-id="0cc47-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="0cc47-119">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0cc47-120">Relações</span><span class="sxs-lookup"><span data-stu-id="0cc47-120">Relationships</span></span>
<span data-ttu-id="0cc47-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0cc47-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0cc47-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0cc47-122">JSON Representation</span></span>
<span data-ttu-id="0cc47-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0cc47-123">Here is a JSON representation of the resource.</span></span>
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





