---
title: Tipo de recurso mediaContentRatingFrance
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c7ac9e4309f2f6cf97c0caf6faed36f43347d5a8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437219"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="0576c-103">Tipo de recurso mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="0576c-103">mediaContentRatingFrance resource type</span></span>

<span data-ttu-id="0576c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0576c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0576c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0576c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0576c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0576c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0576c-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0576c-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="0576c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0576c-108">Properties</span></span>
|<span data-ttu-id="0576c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0576c-109">Property</span></span>|<span data-ttu-id="0576c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0576c-110">Type</span></span>|<span data-ttu-id="0576c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0576c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0576c-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="0576c-112">movieRating</span></span>|[<span data-ttu-id="0576c-113">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="0576c-113">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="0576c-114">Classificação de filmes selecionada para a França.</span><span class="sxs-lookup"><span data-stu-id="0576c-114">Movies rating selected for France.</span></span> <span data-ttu-id="0576c-115">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="0576c-115">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="0576c-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="0576c-116">tvRating</span></span>|[<span data-ttu-id="0576c-117">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="0576c-117">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="0576c-118">Classificação de TV selecionada para a França.</span><span class="sxs-lookup"><span data-stu-id="0576c-118">TV rating selected for France.</span></span> <span data-ttu-id="0576c-119">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="0576c-119">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0576c-120">Relações</span><span class="sxs-lookup"><span data-stu-id="0576c-120">Relationships</span></span>
<span data-ttu-id="0576c-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0576c-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0576c-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0576c-122">JSON Representation</span></span>
<span data-ttu-id="0576c-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0576c-123">Here is a JSON representation of the resource.</span></span>
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



