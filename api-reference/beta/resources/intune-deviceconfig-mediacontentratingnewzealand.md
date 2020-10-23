---
title: Tipo de recurso mediaContentRatingNewZealand
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cad2826c4b3197a7d0ccba850fa1bf14464daf2c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707168"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="c3e85-103">Tipo de recurso mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="c3e85-103">mediaContentRatingNewZealand resource type</span></span>

<span data-ttu-id="c3e85-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3e85-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3e85-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c3e85-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3e85-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c3e85-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3e85-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c3e85-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c3e85-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c3e85-108">Properties</span></span>
|<span data-ttu-id="c3e85-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3e85-109">Property</span></span>|<span data-ttu-id="c3e85-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3e85-110">Type</span></span>|<span data-ttu-id="c3e85-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3e85-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3e85-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="c3e85-112">movieRating</span></span>|[<span data-ttu-id="c3e85-113">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="c3e85-113">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="c3e85-114">Classificação de filmes selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="c3e85-114">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="c3e85-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="c3e85-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="c3e85-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="c3e85-116">tvRating</span></span>|[<span data-ttu-id="c3e85-117">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c3e85-117">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="c3e85-118">Classificação de TV selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="c3e85-118">TV rating selected for New Zealand.</span></span> <span data-ttu-id="c3e85-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="c3e85-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3e85-120">Relações</span><span class="sxs-lookup"><span data-stu-id="c3e85-120">Relationships</span></span>
<span data-ttu-id="c3e85-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c3e85-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3e85-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c3e85-122">JSON Representation</span></span>
<span data-ttu-id="c3e85-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c3e85-123">Here is a JSON representation of the resource.</span></span>
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





