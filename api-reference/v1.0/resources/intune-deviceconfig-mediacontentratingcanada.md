---
title: Tipo de recurso mediaContentRatingCanada
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c806a284afc3eec0e2439b53711459254227793d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003168"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="1273e-103">Tipo de recurso mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="1273e-103">mediaContentRatingCanada resource type</span></span>

<span data-ttu-id="1273e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1273e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1273e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1273e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1273e-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1273e-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1273e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1273e-107">Properties</span></span>
|<span data-ttu-id="1273e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1273e-108">Property</span></span>|<span data-ttu-id="1273e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1273e-109">Type</span></span>|<span data-ttu-id="1273e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1273e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1273e-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="1273e-111">movieRating</span></span>|[<span data-ttu-id="1273e-112">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="1273e-112">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="1273e-113">Classificação de filmes selecionada para o Canadá.</span><span class="sxs-lookup"><span data-stu-id="1273e-113">Movies rating selected for Canada.</span></span> <span data-ttu-id="1273e-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="1273e-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="1273e-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="1273e-115">tvRating</span></span>|[<span data-ttu-id="1273e-116">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="1273e-116">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="1273e-117">Classificação de TV selecionada para o Canadá.</span><span class="sxs-lookup"><span data-stu-id="1273e-117">TV rating selected for Canada.</span></span> <span data-ttu-id="1273e-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="1273e-118">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1273e-119">Relações</span><span class="sxs-lookup"><span data-stu-id="1273e-119">Relationships</span></span>
<span data-ttu-id="1273e-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1273e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1273e-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1273e-121">JSON Representation</span></span>
<span data-ttu-id="1273e-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1273e-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingCanada"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingCanada",
  "movieRating": "String",
  "tvRating": "String"
}
```









