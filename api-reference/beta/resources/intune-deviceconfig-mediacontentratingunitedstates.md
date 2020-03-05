---
title: Tipo de recurso mediaContentRatingUnitedStates
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6574921d91273ebc07f31d404441c492cf71e0bf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529603"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="1529e-103">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="1529e-103">mediaContentRatingUnitedStates resource type</span></span>

<span data-ttu-id="1529e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="1529e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1529e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1529e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1529e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1529e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1529e-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1529e-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="1529e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1529e-108">Properties</span></span>
|<span data-ttu-id="1529e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1529e-109">Property</span></span>|<span data-ttu-id="1529e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1529e-110">Type</span></span>|<span data-ttu-id="1529e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1529e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1529e-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="1529e-112">movieRating</span></span>|[<span data-ttu-id="1529e-113">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="1529e-113">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="1529e-114">Classificação de filmes selecionada para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="1529e-114">Movies rating selected for United States.</span></span> <span data-ttu-id="1529e-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="1529e-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="1529e-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="1529e-116">tvRating</span></span>|[<span data-ttu-id="1529e-117">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="1529e-117">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="1529e-118">Classificação de TV selecionada para Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="1529e-118">TV rating selected for United States.</span></span> <span data-ttu-id="1529e-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="1529e-119">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1529e-120">Relações</span><span class="sxs-lookup"><span data-stu-id="1529e-120">Relationships</span></span>
<span data-ttu-id="1529e-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1529e-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1529e-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1529e-122">JSON Representation</span></span>
<span data-ttu-id="1529e-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1529e-123">Here is a JSON representation of the resource.</span></span>
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



