---
title: Tipo de recurso mediaContentRatingIreland
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b2da5f800d719558e0ba3990fbb7efb7b9280176
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529623"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="3b519-103">Tipo de recurso mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="3b519-103">mediaContentRatingIreland resource type</span></span>

<span data-ttu-id="3b519-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="3b519-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b519-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3b519-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b519-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b519-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b519-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="3b519-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="3b519-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3b519-108">Properties</span></span>
|<span data-ttu-id="3b519-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b519-109">Property</span></span>|<span data-ttu-id="3b519-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b519-110">Type</span></span>|<span data-ttu-id="3b519-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b519-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b519-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="3b519-112">movieRating</span></span>|[<span data-ttu-id="3b519-113">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="3b519-113">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="3b519-114">Classificação de filmes selecionada para a Irlanda.</span><span class="sxs-lookup"><span data-stu-id="3b519-114">Movies rating selected for Ireland.</span></span> <span data-ttu-id="3b519-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="3b519-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="3b519-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="3b519-116">tvRating</span></span>|[<span data-ttu-id="3b519-117">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="3b519-117">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="3b519-118">Classificação de TV selecionada para a Irlanda.</span><span class="sxs-lookup"><span data-stu-id="3b519-118">TV rating selected for Ireland.</span></span> <span data-ttu-id="3b519-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="3b519-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b519-120">Relações</span><span class="sxs-lookup"><span data-stu-id="3b519-120">Relationships</span></span>
<span data-ttu-id="3b519-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3b519-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b519-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3b519-122">JSON Representation</span></span>
<span data-ttu-id="3b519-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3b519-123">Here is a JSON representation of the resource.</span></span>
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



