---
title: Tipo de recurso mediaContentRatingGermany
description: Ainda não documentado
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f32a6ed59861dce47f5c38f7259b78879bf1681c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42788580"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="4a110-103">Tipo de recurso mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="4a110-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="4a110-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="4a110-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a110-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4a110-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a110-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4a110-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="4a110-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a110-107">Properties</span></span>
|<span data-ttu-id="4a110-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a110-108">Property</span></span>|<span data-ttu-id="4a110-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a110-109">Type</span></span>|<span data-ttu-id="4a110-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a110-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a110-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="4a110-111">movieRating</span></span>|[<span data-ttu-id="4a110-112">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="4a110-112">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="4a110-113">Classificação de filmes selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="4a110-113">Movies rating selected for Germany.</span></span> <span data-ttu-id="4a110-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="4a110-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="4a110-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="4a110-115">tvRating</span></span>|[<span data-ttu-id="4a110-116">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="4a110-116">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="4a110-117">Classificação de TV selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="4a110-117">TV rating selected for Germany.</span></span> <span data-ttu-id="4a110-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="4a110-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a110-119">Relações</span><span class="sxs-lookup"><span data-stu-id="4a110-119">Relationships</span></span>
<span data-ttu-id="4a110-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4a110-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4a110-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a110-121">JSON Representation</span></span>
<span data-ttu-id="4a110-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4a110-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```



