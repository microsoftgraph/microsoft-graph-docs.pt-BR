---
title: Tipo de recurso mediaContentRatingCanada
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 424fc81f45848b2872986b4c12efcd8ed995a774
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368769"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="5b1b0-103">Tipo de recurso mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="5b1b0-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="5b1b0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5b1b0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b1b0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5b1b0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b1b0-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5b1b0-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="5b1b0-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5b1b0-107">Properties</span></span>
|<span data-ttu-id="5b1b0-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b1b0-108">Property</span></span>|<span data-ttu-id="5b1b0-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b1b0-109">Type</span></span>|<span data-ttu-id="5b1b0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b1b0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b1b0-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="5b1b0-111">movieRating</span></span>|[<span data-ttu-id="5b1b0-112">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="5b1b0-112">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="5b1b0-113">Classificação de filmes selecionada para o Canadá.</span><span class="sxs-lookup"><span data-stu-id="5b1b0-113">Movies rating selected for Canada.</span></span> <span data-ttu-id="5b1b0-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="5b1b0-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="5b1b0-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="5b1b0-115">tvRating</span></span>|[<span data-ttu-id="5b1b0-116">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="5b1b0-116">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="5b1b0-117">Classificação de TV selecionada para o Canadá.</span><span class="sxs-lookup"><span data-stu-id="5b1b0-117">TV rating selected for Canada.</span></span> <span data-ttu-id="5b1b0-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="5b1b0-118">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b1b0-119">Relações</span><span class="sxs-lookup"><span data-stu-id="5b1b0-119">Relationships</span></span>
<span data-ttu-id="5b1b0-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5b1b0-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b1b0-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5b1b0-121">JSON Representation</span></span>
<span data-ttu-id="5b1b0-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5b1b0-122">Here is a JSON representation of the resource.</span></span>
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



