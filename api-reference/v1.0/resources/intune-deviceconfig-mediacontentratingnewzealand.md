---
title: Tipo de recurso mediaContentRatingNewZealand
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 943a2d12ea1774bff6f12acd958b22f884cfa749
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532438"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="93ff8-103">Tipo de recurso mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="93ff8-103">mediaContentRatingNewZealand resource type</span></span>

<span data-ttu-id="93ff8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93ff8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93ff8-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="93ff8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93ff8-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="93ff8-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="93ff8-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="93ff8-107">Properties</span></span>
|<span data-ttu-id="93ff8-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93ff8-108">Property</span></span>|<span data-ttu-id="93ff8-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="93ff8-109">Type</span></span>|<span data-ttu-id="93ff8-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="93ff8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93ff8-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="93ff8-111">movieRating</span></span>|[<span data-ttu-id="93ff8-112">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="93ff8-112">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="93ff8-113">Classificação de filmes selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="93ff8-113">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="93ff8-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="93ff8-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="93ff8-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="93ff8-115">tvRating</span></span>|[<span data-ttu-id="93ff8-116">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="93ff8-116">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="93ff8-117">Classificação de TV selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="93ff8-117">TV rating selected for New Zealand.</span></span> <span data-ttu-id="93ff8-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="93ff8-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93ff8-119">Relações</span><span class="sxs-lookup"><span data-stu-id="93ff8-119">Relationships</span></span>
<span data-ttu-id="93ff8-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="93ff8-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="93ff8-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="93ff8-121">JSON Representation</span></span>
<span data-ttu-id="93ff8-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="93ff8-122">Here is a JSON representation of the resource.</span></span>
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




