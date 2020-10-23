---
title: Tipo de recurso mediaContentRatingCanada
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 94d291f417ede3a4357372dddf19d3ad1e08f332
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709982"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="b9d05-103">Tipo de recurso mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="b9d05-103">mediaContentRatingCanada resource type</span></span>

<span data-ttu-id="b9d05-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9d05-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9d05-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b9d05-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9d05-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b9d05-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9d05-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="b9d05-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b9d05-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b9d05-108">Properties</span></span>
|<span data-ttu-id="b9d05-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b9d05-109">Property</span></span>|<span data-ttu-id="b9d05-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="b9d05-110">Type</span></span>|<span data-ttu-id="b9d05-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b9d05-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9d05-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="b9d05-112">movieRating</span></span>|[<span data-ttu-id="b9d05-113">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="b9d05-113">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="b9d05-114">Classificação de filmes selecionada para o Canadá.</span><span class="sxs-lookup"><span data-stu-id="b9d05-114">Movies rating selected for Canada.</span></span> <span data-ttu-id="b9d05-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="b9d05-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="b9d05-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="b9d05-116">tvRating</span></span>|[<span data-ttu-id="b9d05-117">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="b9d05-117">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="b9d05-118">Classificação de TV selecionada para o Canadá.</span><span class="sxs-lookup"><span data-stu-id="b9d05-118">TV rating selected for Canada.</span></span> <span data-ttu-id="b9d05-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="b9d05-119">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b9d05-120">Relações</span><span class="sxs-lookup"><span data-stu-id="b9d05-120">Relationships</span></span>
<span data-ttu-id="b9d05-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b9d05-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b9d05-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b9d05-122">JSON Representation</span></span>
<span data-ttu-id="b9d05-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b9d05-123">Here is a JSON representation of the resource.</span></span>
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





