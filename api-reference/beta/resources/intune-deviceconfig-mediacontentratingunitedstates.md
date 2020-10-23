---
title: Tipo de recurso mediaContentRatingUnitedStates
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9af3916d29bfc3f48ee3d4c04dc17ab1f0fa3045
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707161"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="c1493-103">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="c1493-103">mediaContentRatingUnitedStates resource type</span></span>

<span data-ttu-id="c1493-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1493-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1493-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c1493-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1493-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c1493-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1493-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c1493-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c1493-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c1493-108">Properties</span></span>
|<span data-ttu-id="c1493-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1493-109">Property</span></span>|<span data-ttu-id="c1493-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1493-110">Type</span></span>|<span data-ttu-id="c1493-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1493-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1493-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="c1493-112">movieRating</span></span>|[<span data-ttu-id="c1493-113">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="c1493-113">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="c1493-114">Classificação de filmes selecionada para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="c1493-114">Movies rating selected for United States.</span></span> <span data-ttu-id="c1493-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="c1493-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="c1493-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="c1493-116">tvRating</span></span>|[<span data-ttu-id="c1493-117">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c1493-117">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="c1493-118">Classificação de TV selecionada para Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="c1493-118">TV rating selected for United States.</span></span> <span data-ttu-id="c1493-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="c1493-119">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1493-120">Relações</span><span class="sxs-lookup"><span data-stu-id="c1493-120">Relationships</span></span>
<span data-ttu-id="c1493-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c1493-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1493-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c1493-122">JSON Representation</span></span>
<span data-ttu-id="c1493-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c1493-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```





