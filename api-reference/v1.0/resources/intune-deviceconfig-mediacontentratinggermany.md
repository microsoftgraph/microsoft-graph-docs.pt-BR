---
title: Tipo de recurso mediaContentRatingGermany
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1a08891428edd5fec07308e2ff7e44da49eaea93
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530635"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="113a8-103">Tipo de recurso mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="113a8-103">mediaContentRatingGermany resource type</span></span>

<span data-ttu-id="113a8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="113a8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="113a8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="113a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="113a8-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="113a8-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="113a8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="113a8-107">Properties</span></span>
|<span data-ttu-id="113a8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="113a8-108">Property</span></span>|<span data-ttu-id="113a8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="113a8-109">Type</span></span>|<span data-ttu-id="113a8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="113a8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="113a8-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="113a8-111">movieRating</span></span>|[<span data-ttu-id="113a8-112">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="113a8-112">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="113a8-113">Classificação de filmes selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="113a8-113">Movies rating selected for Germany.</span></span> <span data-ttu-id="113a8-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="113a8-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="113a8-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="113a8-115">tvRating</span></span>|[<span data-ttu-id="113a8-116">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="113a8-116">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="113a8-117">Classificação de TV selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="113a8-117">TV rating selected for Germany.</span></span> <span data-ttu-id="113a8-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="113a8-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="113a8-119">Relações</span><span class="sxs-lookup"><span data-stu-id="113a8-119">Relationships</span></span>
<span data-ttu-id="113a8-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="113a8-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="113a8-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="113a8-121">JSON Representation</span></span>
<span data-ttu-id="113a8-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="113a8-122">Here is a JSON representation of the resource.</span></span>
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




