---
title: Tipo de recurso mediaContentRatingAustralia
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2adea6cf8d9957e04c7248993ee6197dbd28850b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49302821"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="c8a85-103">Tipo de recurso mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="c8a85-103">mediaContentRatingAustralia resource type</span></span>

<span data-ttu-id="c8a85-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c8a85-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c8a85-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c8a85-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8a85-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c8a85-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8a85-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c8a85-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c8a85-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c8a85-108">Properties</span></span>
|<span data-ttu-id="c8a85-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c8a85-109">Property</span></span>|<span data-ttu-id="c8a85-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c8a85-110">Type</span></span>|<span data-ttu-id="c8a85-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8a85-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8a85-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="c8a85-112">movieRating</span></span>|[<span data-ttu-id="c8a85-113">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="c8a85-113">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="c8a85-114">Classificação de filmes selecionada para a Austrália.</span><span class="sxs-lookup"><span data-stu-id="c8a85-114">Movies rating selected for Australia.</span></span> <span data-ttu-id="c8a85-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="c8a85-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="c8a85-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="c8a85-116">tvRating</span></span>|[<span data-ttu-id="c8a85-117">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c8a85-117">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="c8a85-118">Classificação de TV selecionada para a Austrália.</span><span class="sxs-lookup"><span data-stu-id="c8a85-118">TV rating selected for Australia.</span></span> <span data-ttu-id="c8a85-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="c8a85-119">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8a85-120">Relações</span><span class="sxs-lookup"><span data-stu-id="c8a85-120">Relationships</span></span>
<span data-ttu-id="c8a85-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c8a85-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c8a85-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c8a85-122">JSON Representation</span></span>
<span data-ttu-id="c8a85-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c8a85-123">Here is a JSON representation of the resource.</span></span>
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




