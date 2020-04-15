---
title: Tipo de recurso mediaContentRatingCanada
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 08673417c883c2aa2a8082010a0eaa001ca02004
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43410076"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="4a853-103">Tipo de recurso mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="4a853-103">mediaContentRatingCanada resource type</span></span>

<span data-ttu-id="4a853-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a853-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4a853-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4a853-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a853-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4a853-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="4a853-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a853-107">Properties</span></span>
|<span data-ttu-id="4a853-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a853-108">Property</span></span>|<span data-ttu-id="4a853-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a853-109">Type</span></span>|<span data-ttu-id="4a853-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a853-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a853-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="4a853-111">movieRating</span></span>|[<span data-ttu-id="4a853-112">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="4a853-112">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="4a853-113">Classificação de filmes selecionada para o Canadá.</span><span class="sxs-lookup"><span data-stu-id="4a853-113">Movies rating selected for Canada.</span></span> <span data-ttu-id="4a853-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="4a853-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="4a853-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="4a853-115">tvRating</span></span>|[<span data-ttu-id="4a853-116">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="4a853-116">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="4a853-117">Classificação de TV selecionada para o Canadá.</span><span class="sxs-lookup"><span data-stu-id="4a853-117">TV rating selected for Canada.</span></span> <span data-ttu-id="4a853-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="4a853-118">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a853-119">Relações</span><span class="sxs-lookup"><span data-stu-id="4a853-119">Relationships</span></span>
<span data-ttu-id="4a853-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4a853-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a853-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a853-121">JSON Representation</span></span>
<span data-ttu-id="4a853-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4a853-122">Here is a JSON representation of the resource.</span></span>
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







