---
title: Tipo de recurso mediaContentRatingAustralia
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eb1cfcafca5b369d8c68103be0795c54842d083f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52742871"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="e8719-103">Tipo de recurso mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="e8719-103">mediaContentRatingAustralia resource type</span></span>

<span data-ttu-id="e8719-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8719-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8719-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e8719-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8719-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="e8719-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e8719-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e8719-107">Properties</span></span>
|<span data-ttu-id="e8719-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e8719-108">Property</span></span>|<span data-ttu-id="e8719-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="e8719-109">Type</span></span>|<span data-ttu-id="e8719-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e8719-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8719-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="e8719-111">movieRating</span></span>|[<span data-ttu-id="e8719-112">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="e8719-112">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="e8719-113">Classificação de filmes selecionada para a Austrália.</span><span class="sxs-lookup"><span data-stu-id="e8719-113">Movies rating selected for Australia.</span></span> <span data-ttu-id="e8719-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="e8719-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="e8719-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="e8719-115">tvRating</span></span>|[<span data-ttu-id="e8719-116">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="e8719-116">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="e8719-117">Classificação de TV selecionada para a Austrália.</span><span class="sxs-lookup"><span data-stu-id="e8719-117">TV rating selected for Australia.</span></span> <span data-ttu-id="e8719-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="e8719-118">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8719-119">Relações</span><span class="sxs-lookup"><span data-stu-id="e8719-119">Relationships</span></span>
<span data-ttu-id="e8719-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="e8719-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8719-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e8719-121">JSON Representation</span></span>
<span data-ttu-id="e8719-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e8719-122">Here is a JSON representation of the resource.</span></span>
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




