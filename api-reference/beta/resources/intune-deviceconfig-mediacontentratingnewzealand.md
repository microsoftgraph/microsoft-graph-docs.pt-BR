---
title: Tipo de recurso mediaContentRatingNewZealand
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4eb72612c61bfe90a6c7071f8645c3471bdd5be5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437159"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="f11d6-103">Tipo de recurso mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="f11d6-103">mediaContentRatingNewZealand resource type</span></span>

<span data-ttu-id="f11d6-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f11d6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f11d6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f11d6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f11d6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f11d6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f11d6-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f11d6-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f11d6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f11d6-108">Properties</span></span>
|<span data-ttu-id="f11d6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f11d6-109">Property</span></span>|<span data-ttu-id="f11d6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f11d6-110">Type</span></span>|<span data-ttu-id="f11d6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f11d6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f11d6-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="f11d6-112">movieRating</span></span>|[<span data-ttu-id="f11d6-113">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="f11d6-113">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="f11d6-114">Classificação de filmes selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="f11d6-114">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="f11d6-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="f11d6-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="f11d6-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="f11d6-116">tvRating</span></span>|[<span data-ttu-id="f11d6-117">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="f11d6-117">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="f11d6-118">Classificação de TV selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="f11d6-118">TV rating selected for New Zealand.</span></span> <span data-ttu-id="f11d6-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="f11d6-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f11d6-120">Relações</span><span class="sxs-lookup"><span data-stu-id="f11d6-120">Relationships</span></span>
<span data-ttu-id="f11d6-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f11d6-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f11d6-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f11d6-122">JSON Representation</span></span>
<span data-ttu-id="f11d6-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f11d6-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingNewZealand"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingNewZealand",
  "movieRating": "String",
  "tvRating": "String"
}
```



