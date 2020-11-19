---
title: Tipo de recurso mediaContentRatingIreland
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 716c840a2fa4254c4f0a4cac9ea32117dc5f279c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268465"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="56c81-103">Tipo de recurso mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="56c81-103">mediaContentRatingIreland resource type</span></span>

<span data-ttu-id="56c81-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56c81-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56c81-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="56c81-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="56c81-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="56c81-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56c81-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="56c81-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="56c81-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="56c81-108">Properties</span></span>
|<span data-ttu-id="56c81-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="56c81-109">Property</span></span>|<span data-ttu-id="56c81-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="56c81-110">Type</span></span>|<span data-ttu-id="56c81-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="56c81-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56c81-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="56c81-112">movieRating</span></span>|[<span data-ttu-id="56c81-113">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="56c81-113">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="56c81-114">Classificação de filmes selecionada para a Irlanda.</span><span class="sxs-lookup"><span data-stu-id="56c81-114">Movies rating selected for Ireland.</span></span> <span data-ttu-id="56c81-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="56c81-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="56c81-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="56c81-116">tvRating</span></span>|[<span data-ttu-id="56c81-117">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="56c81-117">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="56c81-118">Classificação de TV selecionada para a Irlanda.</span><span class="sxs-lookup"><span data-stu-id="56c81-118">TV rating selected for Ireland.</span></span> <span data-ttu-id="56c81-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="56c81-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56c81-120">Relações</span><span class="sxs-lookup"><span data-stu-id="56c81-120">Relationships</span></span>
<span data-ttu-id="56c81-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="56c81-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56c81-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="56c81-122">JSON Representation</span></span>
<span data-ttu-id="56c81-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="56c81-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```




