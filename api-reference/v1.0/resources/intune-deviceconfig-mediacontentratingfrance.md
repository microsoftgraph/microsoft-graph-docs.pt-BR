---
title: Tipo de recurso mediaContentRatingFrance
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 44b6374d4831ca0b3b220f237a3c8d9938df18e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003140"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="cca35-103">Tipo de recurso mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="cca35-103">mediaContentRatingFrance resource type</span></span>

<span data-ttu-id="cca35-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cca35-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cca35-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cca35-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cca35-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cca35-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="cca35-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cca35-107">Properties</span></span>
|<span data-ttu-id="cca35-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cca35-108">Property</span></span>|<span data-ttu-id="cca35-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="cca35-109">Type</span></span>|<span data-ttu-id="cca35-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cca35-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cca35-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="cca35-111">movieRating</span></span>|[<span data-ttu-id="cca35-112">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="cca35-112">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="cca35-113">Classificação de filmes selecionada para a França.</span><span class="sxs-lookup"><span data-stu-id="cca35-113">Movies rating selected for France.</span></span> <span data-ttu-id="cca35-114">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="cca35-114">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="cca35-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="cca35-115">tvRating</span></span>|[<span data-ttu-id="cca35-116">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="cca35-116">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="cca35-117">Classificação de TV selecionada para a França.</span><span class="sxs-lookup"><span data-stu-id="cca35-117">TV rating selected for France.</span></span> <span data-ttu-id="cca35-118">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="cca35-118">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cca35-119">Relações</span><span class="sxs-lookup"><span data-stu-id="cca35-119">Relationships</span></span>
<span data-ttu-id="cca35-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cca35-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cca35-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cca35-121">JSON Representation</span></span>
<span data-ttu-id="cca35-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cca35-122">Here is a JSON representation of the resource.</span></span>
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









