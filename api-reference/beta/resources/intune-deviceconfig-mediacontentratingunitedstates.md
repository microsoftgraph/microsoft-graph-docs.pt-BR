---
title: Tipo de recurso mediaContentRatingUnitedStates
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7ccfd31d7e47d4a4e08a63e163661c4a2a82da7c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052695"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="d0359-103">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="d0359-103">mediaContentRatingUnitedStates resource type</span></span>

<span data-ttu-id="d0359-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0359-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d0359-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d0359-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0359-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d0359-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0359-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d0359-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d0359-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d0359-108">Properties</span></span>
|<span data-ttu-id="d0359-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d0359-109">Property</span></span>|<span data-ttu-id="d0359-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d0359-110">Type</span></span>|<span data-ttu-id="d0359-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d0359-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0359-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="d0359-112">movieRating</span></span>|[<span data-ttu-id="d0359-113">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="d0359-113">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="d0359-114">Classificação de filmes selecionada para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="d0359-114">Movies rating selected for United States.</span></span> <span data-ttu-id="d0359-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="d0359-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="d0359-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="d0359-116">tvRating</span></span>|[<span data-ttu-id="d0359-117">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="d0359-117">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="d0359-118">Classificação de TV selecionada para Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="d0359-118">TV rating selected for United States.</span></span> <span data-ttu-id="d0359-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="d0359-119">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0359-120">Relações</span><span class="sxs-lookup"><span data-stu-id="d0359-120">Relationships</span></span>
<span data-ttu-id="d0359-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d0359-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0359-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d0359-122">JSON Representation</span></span>
<span data-ttu-id="d0359-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d0359-123">Here is a JSON representation of the resource.</span></span>
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






