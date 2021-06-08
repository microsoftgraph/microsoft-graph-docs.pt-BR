---
title: Tipo de recurso mediaContentRatingNewZealand
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4fc7374d8e71714a5c66da1b2dc66aa5175c3e33
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760248"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="79559-103">Tipo de recurso mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="79559-103">mediaContentRatingNewZealand resource type</span></span>

<span data-ttu-id="79559-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="79559-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="79559-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="79559-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79559-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="79559-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="79559-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79559-107">Properties</span></span>
|<span data-ttu-id="79559-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79559-108">Property</span></span>|<span data-ttu-id="79559-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="79559-109">Type</span></span>|<span data-ttu-id="79559-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="79559-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79559-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="79559-111">movieRating</span></span>|[<span data-ttu-id="79559-112">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="79559-112">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="79559-113">Classificação de filmes selecionada para a Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="79559-113">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="79559-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="79559-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="79559-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="79559-115">tvRating</span></span>|[<span data-ttu-id="79559-116">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="79559-116">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="79559-117">Classificação de TV selecionada para a Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="79559-117">TV rating selected for New Zealand.</span></span> <span data-ttu-id="79559-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="79559-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79559-119">Relações</span><span class="sxs-lookup"><span data-stu-id="79559-119">Relationships</span></span>
<span data-ttu-id="79559-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="79559-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="79559-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79559-121">JSON Representation</span></span>
<span data-ttu-id="79559-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="79559-122">Here is a JSON representation of the resource.</span></span>
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




