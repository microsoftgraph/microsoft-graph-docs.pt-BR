---
title: Tipo de recurso mediaContentRatingAustralia
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 973c8abcbb2cc0cdc523fc4175282c523266b58c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42418150"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="5ae2b-103">Tipo de recurso mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="5ae2b-103">mediaContentRatingAustralia resource type</span></span>

<span data-ttu-id="5ae2b-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="5ae2b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ae2b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5ae2b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ae2b-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5ae2b-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="5ae2b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5ae2b-107">Properties</span></span>
|<span data-ttu-id="5ae2b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ae2b-108">Property</span></span>|<span data-ttu-id="5ae2b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ae2b-109">Type</span></span>|<span data-ttu-id="5ae2b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ae2b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ae2b-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="5ae2b-111">movieRating</span></span>|[<span data-ttu-id="5ae2b-112">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="5ae2b-112">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="5ae2b-113">Classificação de filmes selecionada para a Austrália.</span><span class="sxs-lookup"><span data-stu-id="5ae2b-113">Movies rating selected for Australia.</span></span> <span data-ttu-id="5ae2b-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="5ae2b-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="5ae2b-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="5ae2b-115">tvRating</span></span>|[<span data-ttu-id="5ae2b-116">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="5ae2b-116">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="5ae2b-117">Classificação de TV selecionada para a Austrália.</span><span class="sxs-lookup"><span data-stu-id="5ae2b-117">TV rating selected for Australia.</span></span> <span data-ttu-id="5ae2b-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="5ae2b-118">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ae2b-119">Relações</span><span class="sxs-lookup"><span data-stu-id="5ae2b-119">Relationships</span></span>
<span data-ttu-id="5ae2b-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5ae2b-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ae2b-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5ae2b-121">JSON Representation</span></span>
<span data-ttu-id="5ae2b-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5ae2b-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```




