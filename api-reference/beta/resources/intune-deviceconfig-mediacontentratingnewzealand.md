---
title: Tipo de recurso mediaContentRatingNewZealand
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b9d8ab3fa54e9c173cfe41b6c4462df38daef0f3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273449"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="cdedd-103">Tipo de recurso mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="cdedd-103">mediaContentRatingNewZealand resource type</span></span>

<span data-ttu-id="cdedd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdedd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cdedd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cdedd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdedd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cdedd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdedd-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cdedd-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="cdedd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cdedd-108">Properties</span></span>
|<span data-ttu-id="cdedd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cdedd-109">Property</span></span>|<span data-ttu-id="cdedd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cdedd-110">Type</span></span>|<span data-ttu-id="cdedd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdedd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdedd-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="cdedd-112">movieRating</span></span>|[<span data-ttu-id="cdedd-113">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="cdedd-113">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="cdedd-114">Classificação de filmes selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="cdedd-114">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="cdedd-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="cdedd-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="cdedd-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="cdedd-116">tvRating</span></span>|[<span data-ttu-id="cdedd-117">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="cdedd-117">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="cdedd-118">Classificação de TV selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="cdedd-118">TV rating selected for New Zealand.</span></span> <span data-ttu-id="cdedd-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="cdedd-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cdedd-120">Relações</span><span class="sxs-lookup"><span data-stu-id="cdedd-120">Relationships</span></span>
<span data-ttu-id="cdedd-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cdedd-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cdedd-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cdedd-122">JSON Representation</span></span>
<span data-ttu-id="cdedd-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cdedd-123">Here is a JSON representation of the resource.</span></span>
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




