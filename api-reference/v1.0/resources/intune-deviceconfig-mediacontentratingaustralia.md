---
title: Tipo de recurso mediaContentRatingAustralia
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0a9e3035585794216440522233f23a8061ddafee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031427"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="0dddb-103">Tipo de recurso mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="0dddb-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="0dddb-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0dddb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0dddb-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0dddb-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="0dddb-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0dddb-106">Properties</span></span>
|<span data-ttu-id="0dddb-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0dddb-107">Property</span></span>|<span data-ttu-id="0dddb-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0dddb-108">Type</span></span>|<span data-ttu-id="0dddb-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0dddb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0dddb-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="0dddb-110">movieRating</span></span>|[<span data-ttu-id="0dddb-111">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="0dddb-111">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="0dddb-112">Classificação de filmes selecionada para a Austrália.</span><span class="sxs-lookup"><span data-stu-id="0dddb-112">Movies rating selected for Australia.</span></span> <span data-ttu-id="0dddb-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="0dddb-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="0dddb-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="0dddb-114">tvRating</span></span>|[<span data-ttu-id="0dddb-115">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="0dddb-115">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="0dddb-116">Classificação de TV selecionada para a Austrália.</span><span class="sxs-lookup"><span data-stu-id="0dddb-116">TV rating selected for Australia.</span></span> <span data-ttu-id="0dddb-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="0dddb-117">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0dddb-118">Relações</span><span class="sxs-lookup"><span data-stu-id="0dddb-118">Relationships</span></span>
<span data-ttu-id="0dddb-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0dddb-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0dddb-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0dddb-120">JSON Representation</span></span>
<span data-ttu-id="0dddb-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0dddb-121">Here is a JSON representation of the resource.</span></span>
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



