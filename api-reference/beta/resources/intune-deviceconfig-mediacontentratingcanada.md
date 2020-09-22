---
title: Tipo de recurso mediaContentRatingCanada
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f0e35a13285ffa1cb134ea4b87928fd690ca9c21
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989315"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="51d87-103">Tipo de recurso mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="51d87-103">mediaContentRatingCanada resource type</span></span>

<span data-ttu-id="51d87-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51d87-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51d87-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="51d87-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51d87-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="51d87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51d87-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="51d87-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="51d87-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="51d87-108">Properties</span></span>
|<span data-ttu-id="51d87-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51d87-109">Property</span></span>|<span data-ttu-id="51d87-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="51d87-110">Type</span></span>|<span data-ttu-id="51d87-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="51d87-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51d87-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="51d87-112">movieRating</span></span>|[<span data-ttu-id="51d87-113">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="51d87-113">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="51d87-114">Classificação de filmes selecionada para o Canadá.</span><span class="sxs-lookup"><span data-stu-id="51d87-114">Movies rating selected for Canada.</span></span> <span data-ttu-id="51d87-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="51d87-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="51d87-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="51d87-116">tvRating</span></span>|[<span data-ttu-id="51d87-117">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="51d87-117">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="51d87-118">Classificação de TV selecionada para o Canadá.</span><span class="sxs-lookup"><span data-stu-id="51d87-118">TV rating selected for Canada.</span></span> <span data-ttu-id="51d87-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="51d87-119">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51d87-120">Relações</span><span class="sxs-lookup"><span data-stu-id="51d87-120">Relationships</span></span>
<span data-ttu-id="51d87-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="51d87-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="51d87-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="51d87-122">JSON Representation</span></span>
<span data-ttu-id="51d87-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="51d87-123">Here is a JSON representation of the resource.</span></span>
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






