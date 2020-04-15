---
title: Tipo de recurso mediaContentRatingGermany
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3adb081f2b18bbf38327cd56adf90f29333ec146
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439446"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="7e139-103">Tipo de recurso mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="7e139-103">mediaContentRatingGermany resource type</span></span>

<span data-ttu-id="7e139-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7e139-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e139-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7e139-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e139-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7e139-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="7e139-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7e139-107">Properties</span></span>
|<span data-ttu-id="7e139-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7e139-108">Property</span></span>|<span data-ttu-id="7e139-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7e139-109">Type</span></span>|<span data-ttu-id="7e139-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7e139-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e139-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="7e139-111">movieRating</span></span>|[<span data-ttu-id="7e139-112">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="7e139-112">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="7e139-113">Classificação de filmes selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="7e139-113">Movies rating selected for Germany.</span></span> <span data-ttu-id="7e139-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="7e139-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="7e139-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="7e139-115">tvRating</span></span>|[<span data-ttu-id="7e139-116">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="7e139-116">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="7e139-117">Classificação de TV selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="7e139-117">TV rating selected for Germany.</span></span> <span data-ttu-id="7e139-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="7e139-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e139-119">Relações</span><span class="sxs-lookup"><span data-stu-id="7e139-119">Relationships</span></span>
<span data-ttu-id="7e139-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7e139-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e139-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7e139-121">JSON Representation</span></span>
<span data-ttu-id="7e139-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7e139-122">Here is a JSON representation of the resource.</span></span>
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







