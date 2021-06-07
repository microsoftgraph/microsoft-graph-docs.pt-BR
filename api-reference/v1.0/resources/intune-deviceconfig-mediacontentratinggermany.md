---
title: Tipo de recurso mediaContentRatingGermany
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 06cad29f595ecc1124344d2ad72bed50a71b4314
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757763"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="e3f82-103">Tipo de recurso mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="e3f82-103">mediaContentRatingGermany resource type</span></span>

<span data-ttu-id="e3f82-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3f82-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3f82-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e3f82-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3f82-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e3f82-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e3f82-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e3f82-107">Properties</span></span>
|<span data-ttu-id="e3f82-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e3f82-108">Property</span></span>|<span data-ttu-id="e3f82-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e3f82-109">Type</span></span>|<span data-ttu-id="e3f82-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3f82-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3f82-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="e3f82-111">movieRating</span></span>|[<span data-ttu-id="e3f82-112">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="e3f82-112">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="e3f82-113">Classificação de filmes selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="e3f82-113">Movies rating selected for Germany.</span></span> <span data-ttu-id="e3f82-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="e3f82-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="e3f82-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="e3f82-115">tvRating</span></span>|[<span data-ttu-id="e3f82-116">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="e3f82-116">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="e3f82-117">Classificação de TV selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="e3f82-117">TV rating selected for Germany.</span></span> <span data-ttu-id="e3f82-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="e3f82-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3f82-119">Relações</span><span class="sxs-lookup"><span data-stu-id="e3f82-119">Relationships</span></span>
<span data-ttu-id="e3f82-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e3f82-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e3f82-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e3f82-121">JSON Representation</span></span>
<span data-ttu-id="e3f82-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e3f82-122">Here is a JSON representation of the resource.</span></span>
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




