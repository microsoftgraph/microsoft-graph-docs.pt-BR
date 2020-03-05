---
title: Tipo de recurso mediaContentRatingUnitedKingdom
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 485213d59e42793301acfe637554c08d9325b7ad
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526017"
---
# <a name="mediacontentratingunitedkingdom-resource-type"></a><span data-ttu-id="f3600-103">Tipo de recurso mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="f3600-103">mediaContentRatingUnitedKingdom resource type</span></span>

<span data-ttu-id="f3600-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f3600-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3600-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f3600-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3600-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f3600-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3600-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f3600-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f3600-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f3600-108">Properties</span></span>
|<span data-ttu-id="f3600-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3600-109">Property</span></span>|<span data-ttu-id="f3600-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3600-110">Type</span></span>|<span data-ttu-id="f3600-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3600-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3600-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="f3600-112">movieRating</span></span>|[<span data-ttu-id="f3600-113">ratingUnitedKingdomMoviesType</span><span class="sxs-lookup"><span data-stu-id="f3600-113">ratingUnitedKingdomMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdommoviestype.md)|<span data-ttu-id="f3600-114">Classificação de filmes selecionada para o Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="f3600-114">Movies rating selected for United Kingdom.</span></span> <span data-ttu-id="f3600-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="f3600-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `universalChildren`, `parentalGuidance`, `agesAbove12Video`, `agesAbove12Cinema`, `agesAbove15`, `adults`.</span></span>|
|<span data-ttu-id="f3600-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="f3600-116">tvRating</span></span>|[<span data-ttu-id="f3600-117">ratingUnitedKingdomTelevisionType</span><span class="sxs-lookup"><span data-stu-id="f3600-117">ratingUnitedKingdomTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedkingdomtelevisiontype.md)|<span data-ttu-id="f3600-118">Classificação de TV selecionada para o Reino Unido.</span><span class="sxs-lookup"><span data-stu-id="f3600-118">TV rating selected for United Kingdom.</span></span> <span data-ttu-id="f3600-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `caution`.</span><span class="sxs-lookup"><span data-stu-id="f3600-119">Possible values are: `allAllowed`, `allBlocked`, `caution`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3600-120">Relações</span><span class="sxs-lookup"><span data-stu-id="f3600-120">Relationships</span></span>
<span data-ttu-id="f3600-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f3600-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3600-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f3600-122">JSON Representation</span></span>
<span data-ttu-id="f3600-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f3600-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedKingdom",
  "movieRating": "String",
  "tvRating": "String"
}
```



