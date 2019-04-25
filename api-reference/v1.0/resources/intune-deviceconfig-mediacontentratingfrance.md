---
title: Tipo de recurso mediaContentRatingFrance
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 979a5996b655ba13847e52dc09b083169ff0815a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572343"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="dbf87-103">Tipo de recurso mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="dbf87-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="dbf87-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dbf87-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbf87-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="dbf87-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="dbf87-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dbf87-106">Properties</span></span>
|<span data-ttu-id="dbf87-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dbf87-107">Property</span></span>|<span data-ttu-id="dbf87-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbf87-108">Type</span></span>|<span data-ttu-id="dbf87-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbf87-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbf87-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="dbf87-110">movieRating</span></span>|[<span data-ttu-id="dbf87-111">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="dbf87-111">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="dbf87-112">Classificação de filmes selecionada para a França.</span><span class="sxs-lookup"><span data-stu-id="dbf87-112">Movies rating selected for France.</span></span> <span data-ttu-id="dbf87-113">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="dbf87-113">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="dbf87-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="dbf87-114">tvRating</span></span>|[<span data-ttu-id="dbf87-115">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="dbf87-115">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="dbf87-116">Classificação de TV selecionada para a França.</span><span class="sxs-lookup"><span data-stu-id="dbf87-116">TV rating selected for France.</span></span> <span data-ttu-id="dbf87-117">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="dbf87-117">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dbf87-118">Relações</span><span class="sxs-lookup"><span data-stu-id="dbf87-118">Relationships</span></span>
<span data-ttu-id="dbf87-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="dbf87-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dbf87-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dbf87-120">JSON Representation</span></span>
<span data-ttu-id="dbf87-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dbf87-121">Here is a JSON representation of the resource.</span></span>
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



