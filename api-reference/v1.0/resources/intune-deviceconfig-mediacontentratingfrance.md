---
title: Tipo de recurso mediaContentRatingFrance
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 724fe7a511616b457d29cd804c19d69705bfb42b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757770"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="9b8c9-103">Tipo de recurso mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="9b8c9-103">mediaContentRatingFrance resource type</span></span>

<span data-ttu-id="9b8c9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b8c9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b8c9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9b8c9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b8c9-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9b8c9-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9b8c9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9b8c9-107">Properties</span></span>
|<span data-ttu-id="9b8c9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b8c9-108">Property</span></span>|<span data-ttu-id="9b8c9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b8c9-109">Type</span></span>|<span data-ttu-id="9b8c9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b8c9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b8c9-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="9b8c9-111">movieRating</span></span>|[<span data-ttu-id="9b8c9-112">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="9b8c9-112">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="9b8c9-113">Classificação de filmes selecionada para a França.</span><span class="sxs-lookup"><span data-stu-id="9b8c9-113">Movies rating selected for France.</span></span> <span data-ttu-id="9b8c9-114">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="9b8c9-114">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="9b8c9-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="9b8c9-115">tvRating</span></span>|[<span data-ttu-id="9b8c9-116">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="9b8c9-116">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="9b8c9-117">Classificação de TV selecionada para a França.</span><span class="sxs-lookup"><span data-stu-id="9b8c9-117">TV rating selected for France.</span></span> <span data-ttu-id="9b8c9-118">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="9b8c9-118">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b8c9-119">Relações</span><span class="sxs-lookup"><span data-stu-id="9b8c9-119">Relationships</span></span>
<span data-ttu-id="9b8c9-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="9b8c9-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b8c9-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9b8c9-121">JSON Representation</span></span>
<span data-ttu-id="9b8c9-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9b8c9-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```




