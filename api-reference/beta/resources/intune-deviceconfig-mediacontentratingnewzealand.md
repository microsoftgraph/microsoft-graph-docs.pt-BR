---
title: Tipo de recurso mediaContentRatingNewZealand
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c9c225f98bdcf182bf708ac2499bd1bdf004bc1d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529610"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="d26db-103">Tipo de recurso mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="d26db-103">mediaContentRatingNewZealand resource type</span></span>

<span data-ttu-id="d26db-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d26db-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d26db-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d26db-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d26db-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d26db-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d26db-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d26db-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="d26db-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d26db-108">Properties</span></span>
|<span data-ttu-id="d26db-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d26db-109">Property</span></span>|<span data-ttu-id="d26db-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d26db-110">Type</span></span>|<span data-ttu-id="d26db-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d26db-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d26db-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="d26db-112">movieRating</span></span>|[<span data-ttu-id="d26db-113">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="d26db-113">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="d26db-114">Classificação de filmes selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="d26db-114">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="d26db-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="d26db-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="d26db-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="d26db-116">tvRating</span></span>|[<span data-ttu-id="d26db-117">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="d26db-117">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="d26db-118">Classificação de TV selecionada para Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="d26db-118">TV rating selected for New Zealand.</span></span> <span data-ttu-id="d26db-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="d26db-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d26db-120">Relações</span><span class="sxs-lookup"><span data-stu-id="d26db-120">Relationships</span></span>
<span data-ttu-id="d26db-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d26db-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d26db-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d26db-122">JSON Representation</span></span>
<span data-ttu-id="d26db-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d26db-123">Here is a JSON representation of the resource.</span></span>
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



