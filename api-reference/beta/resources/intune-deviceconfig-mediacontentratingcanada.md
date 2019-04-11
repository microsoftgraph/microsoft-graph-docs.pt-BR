---
title: Tipo de recurso mediaContentRatingCanada
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 503218cf76d235f4122e36d1d358dce9a76e0fda
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799703"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="6c259-103">Tipo de recurso mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="6c259-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="6c259-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6c259-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c259-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6c259-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c259-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6c259-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6c259-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6c259-107">Properties</span></span>
|<span data-ttu-id="6c259-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c259-108">Property</span></span>|<span data-ttu-id="6c259-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c259-109">Type</span></span>|<span data-ttu-id="6c259-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c259-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c259-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="6c259-111">movieRating</span></span>|[<span data-ttu-id="6c259-112">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="6c259-112">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="6c259-113">Classificação de filmes selecionada para o Canadá.</span><span class="sxs-lookup"><span data-stu-id="6c259-113">Movies rating selected for Canada.</span></span> <span data-ttu-id="6c259-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="6c259-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="6c259-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="6c259-115">tvRating</span></span>|[<span data-ttu-id="6c259-116">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="6c259-116">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="6c259-117">Classificação de TV selecionada para o Canadá.</span><span class="sxs-lookup"><span data-stu-id="6c259-117">TV rating selected for Canada.</span></span> <span data-ttu-id="6c259-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="6c259-118">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c259-119">Relações</span><span class="sxs-lookup"><span data-stu-id="6c259-119">Relationships</span></span>
<span data-ttu-id="6c259-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="6c259-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c259-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6c259-121">JSON Representation</span></span>
<span data-ttu-id="6c259-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6c259-122">Here is a JSON representation of the resource.</span></span>
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





