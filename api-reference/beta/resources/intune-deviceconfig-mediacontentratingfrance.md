---
title: Tipo de recurso mediaContentRatingFrance
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1ea96fd380f7ee7b859e812c51c0620d31742790
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268479"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="d8e12-103">Tipo de recurso mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="d8e12-103">mediaContentRatingFrance resource type</span></span>

<span data-ttu-id="d8e12-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8e12-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8e12-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d8e12-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8e12-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d8e12-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8e12-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d8e12-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d8e12-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8e12-108">Properties</span></span>
|<span data-ttu-id="d8e12-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8e12-109">Property</span></span>|<span data-ttu-id="d8e12-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8e12-110">Type</span></span>|<span data-ttu-id="d8e12-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8e12-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8e12-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="d8e12-112">movieRating</span></span>|[<span data-ttu-id="d8e12-113">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="d8e12-113">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="d8e12-114">Classificação de filmes selecionada para a França.</span><span class="sxs-lookup"><span data-stu-id="d8e12-114">Movies rating selected for France.</span></span> <span data-ttu-id="d8e12-115">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="d8e12-115">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="d8e12-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="d8e12-116">tvRating</span></span>|[<span data-ttu-id="d8e12-117">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="d8e12-117">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="d8e12-118">Classificação de TV selecionada para a França.</span><span class="sxs-lookup"><span data-stu-id="d8e12-118">TV rating selected for France.</span></span> <span data-ttu-id="d8e12-119">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="d8e12-119">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8e12-120">Relações</span><span class="sxs-lookup"><span data-stu-id="d8e12-120">Relationships</span></span>
<span data-ttu-id="d8e12-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d8e12-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8e12-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8e12-122">JSON Representation</span></span>
<span data-ttu-id="d8e12-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d8e12-123">Here is a JSON representation of the resource.</span></span>
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




