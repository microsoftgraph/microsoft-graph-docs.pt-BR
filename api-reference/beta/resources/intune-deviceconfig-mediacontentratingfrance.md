---
title: Tipo de recurso mediaContentRatingFrance
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9ef83c2b02832f46a85a4d2605fdad62f7a42a19
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48702471"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="64d1a-103">Tipo de recurso mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="64d1a-103">mediaContentRatingFrance resource type</span></span>

<span data-ttu-id="64d1a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="64d1a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="64d1a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="64d1a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="64d1a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="64d1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="64d1a-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="64d1a-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="64d1a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="64d1a-108">Properties</span></span>
|<span data-ttu-id="64d1a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="64d1a-109">Property</span></span>|<span data-ttu-id="64d1a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="64d1a-110">Type</span></span>|<span data-ttu-id="64d1a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="64d1a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64d1a-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="64d1a-112">movieRating</span></span>|[<span data-ttu-id="64d1a-113">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="64d1a-113">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="64d1a-114">Classificação de filmes selecionada para a França.</span><span class="sxs-lookup"><span data-stu-id="64d1a-114">Movies rating selected for France.</span></span> <span data-ttu-id="64d1a-115">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="64d1a-115">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="64d1a-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="64d1a-116">tvRating</span></span>|[<span data-ttu-id="64d1a-117">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="64d1a-117">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="64d1a-118">Classificação de TV selecionada para a França.</span><span class="sxs-lookup"><span data-stu-id="64d1a-118">TV rating selected for France.</span></span> <span data-ttu-id="64d1a-119">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="64d1a-119">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64d1a-120">Relações</span><span class="sxs-lookup"><span data-stu-id="64d1a-120">Relationships</span></span>
<span data-ttu-id="64d1a-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="64d1a-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="64d1a-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="64d1a-122">JSON Representation</span></span>
<span data-ttu-id="64d1a-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="64d1a-123">Here is a JSON representation of the resource.</span></span>
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





