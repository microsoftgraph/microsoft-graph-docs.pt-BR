---
title: Tipo de recurso mediaContentRatingAustralia
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 878aa40d55f9c902e8f243d4839ea62cecfe1809
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437241"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="d9f1a-103">Tipo de recurso mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="d9f1a-103">mediaContentRatingAustralia resource type</span></span>

<span data-ttu-id="d9f1a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9f1a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d9f1a-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d9f1a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9f1a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9f1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9f1a-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d9f1a-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d9f1a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d9f1a-108">Properties</span></span>
|<span data-ttu-id="d9f1a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9f1a-109">Property</span></span>|<span data-ttu-id="d9f1a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9f1a-110">Type</span></span>|<span data-ttu-id="d9f1a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9f1a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9f1a-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="d9f1a-112">movieRating</span></span>|[<span data-ttu-id="d9f1a-113">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="d9f1a-113">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="d9f1a-114">Classificação de filmes selecionada para a Austrália.</span><span class="sxs-lookup"><span data-stu-id="d9f1a-114">Movies rating selected for Australia.</span></span> <span data-ttu-id="d9f1a-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="d9f1a-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="d9f1a-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="d9f1a-116">tvRating</span></span>|[<span data-ttu-id="d9f1a-117">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="d9f1a-117">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="d9f1a-118">Classificação de TV selecionada para a Austrália.</span><span class="sxs-lookup"><span data-stu-id="d9f1a-118">TV rating selected for Australia.</span></span> <span data-ttu-id="d9f1a-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="d9f1a-119">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9f1a-120">Relações</span><span class="sxs-lookup"><span data-stu-id="d9f1a-120">Relationships</span></span>
<span data-ttu-id="d9f1a-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d9f1a-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9f1a-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d9f1a-122">JSON Representation</span></span>
<span data-ttu-id="d9f1a-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d9f1a-123">Here is a JSON representation of the resource.</span></span>
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



