---
title: Tipo de recurso mediaContentRatingNewZealand
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e61d2b5e9589bd0e337941dfce7cc1bfbbbc8dd4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788559"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="57115-103">Tipo de recurso mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="57115-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="57115-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="57115-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57115-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="57115-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57115-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="57115-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="57115-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="57115-107">Properties</span></span>
|<span data-ttu-id="57115-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57115-108">Property</span></span>|<span data-ttu-id="57115-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="57115-109">Type</span></span>|<span data-ttu-id="57115-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="57115-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57115-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="57115-111">movieRating</span></span>|[<span data-ttu-id="57115-112">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="57115-112">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="57115-113">Classificação de filmes selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="57115-113">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="57115-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="57115-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="57115-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="57115-115">tvRating</span></span>|[<span data-ttu-id="57115-116">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="57115-116">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="57115-117">Classificação de TV selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="57115-117">TV rating selected for New Zealand.</span></span> <span data-ttu-id="57115-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="57115-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57115-119">Relações</span><span class="sxs-lookup"><span data-stu-id="57115-119">Relationships</span></span>
<span data-ttu-id="57115-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="57115-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57115-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="57115-121">JSON Representation</span></span>
<span data-ttu-id="57115-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="57115-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```



