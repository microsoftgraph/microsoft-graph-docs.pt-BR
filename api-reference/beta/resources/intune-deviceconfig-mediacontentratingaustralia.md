---
title: Tipo de recurso mediaContentRatingAustralia
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f16db693a751641c1b03692f0500cd5dc6d3bfc8
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48709983"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="df101-103">Tipo de recurso mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="df101-103">mediaContentRatingAustralia resource type</span></span>

<span data-ttu-id="df101-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df101-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="df101-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="df101-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df101-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="df101-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df101-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="df101-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="df101-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df101-108">Properties</span></span>
|<span data-ttu-id="df101-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df101-109">Property</span></span>|<span data-ttu-id="df101-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="df101-110">Type</span></span>|<span data-ttu-id="df101-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="df101-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df101-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="df101-112">movieRating</span></span>|[<span data-ttu-id="df101-113">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="df101-113">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="df101-114">Classificação de filmes selecionada para a Austrália.</span><span class="sxs-lookup"><span data-stu-id="df101-114">Movies rating selected for Australia.</span></span> <span data-ttu-id="df101-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="df101-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="df101-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="df101-116">tvRating</span></span>|[<span data-ttu-id="df101-117">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="df101-117">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="df101-118">Classificação de TV selecionada para a Austrália.</span><span class="sxs-lookup"><span data-stu-id="df101-118">TV rating selected for Australia.</span></span> <span data-ttu-id="df101-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="df101-119">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="df101-120">Relações</span><span class="sxs-lookup"><span data-stu-id="df101-120">Relationships</span></span>
<span data-ttu-id="df101-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="df101-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="df101-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="df101-122">JSON Representation</span></span>
<span data-ttu-id="df101-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="df101-123">Here is a JSON representation of the resource.</span></span>
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





