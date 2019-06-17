---
title: Tipo de recurso mediaContentRatingNewZealand
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c69f2d22494e23783c39d781fee28ece49241b52
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34986757"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="7dd93-103">Tipo de recurso mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="7dd93-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="7dd93-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7dd93-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7dd93-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7dd93-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7dd93-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7dd93-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="7dd93-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7dd93-107">Properties</span></span>
|<span data-ttu-id="7dd93-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7dd93-108">Property</span></span>|<span data-ttu-id="7dd93-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7dd93-109">Type</span></span>|<span data-ttu-id="7dd93-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7dd93-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dd93-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="7dd93-111">movieRating</span></span>|[<span data-ttu-id="7dd93-112">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="7dd93-112">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="7dd93-113">Classificação de filmes selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="7dd93-113">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="7dd93-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="7dd93-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="7dd93-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="7dd93-115">tvRating</span></span>|[<span data-ttu-id="7dd93-116">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="7dd93-116">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="7dd93-117">Classificação de TV selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="7dd93-117">TV rating selected for New Zealand.</span></span> <span data-ttu-id="7dd93-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="7dd93-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7dd93-119">Relações</span><span class="sxs-lookup"><span data-stu-id="7dd93-119">Relationships</span></span>
<span data-ttu-id="7dd93-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7dd93-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7dd93-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7dd93-121">JSON Representation</span></span>
<span data-ttu-id="7dd93-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7dd93-122">Here is a JSON representation of the resource.</span></span>
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





