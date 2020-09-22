---
title: Tipo de recurso mediaContentRatingNewZealand
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 252f96785a9e5e19c4b7a19f962c856688339050
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993767"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="52910-103">Tipo de recurso mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="52910-103">mediaContentRatingNewZealand resource type</span></span>

<span data-ttu-id="52910-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52910-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52910-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="52910-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52910-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="52910-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52910-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="52910-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="52910-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52910-108">Properties</span></span>
|<span data-ttu-id="52910-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52910-109">Property</span></span>|<span data-ttu-id="52910-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="52910-110">Type</span></span>|<span data-ttu-id="52910-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="52910-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52910-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="52910-112">movieRating</span></span>|[<span data-ttu-id="52910-113">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="52910-113">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="52910-114">Classificação de filmes selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="52910-114">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="52910-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="52910-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="52910-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="52910-116">tvRating</span></span>|[<span data-ttu-id="52910-117">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="52910-117">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="52910-118">Classificação de TV selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="52910-118">TV rating selected for New Zealand.</span></span> <span data-ttu-id="52910-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="52910-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52910-120">Relações</span><span class="sxs-lookup"><span data-stu-id="52910-120">Relationships</span></span>
<span data-ttu-id="52910-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="52910-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="52910-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52910-122">JSON Representation</span></span>
<span data-ttu-id="52910-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52910-123">Here is a JSON representation of the resource.</span></span>
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






