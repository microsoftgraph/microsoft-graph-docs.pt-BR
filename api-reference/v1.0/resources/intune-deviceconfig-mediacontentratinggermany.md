---
title: Tipo de recurso mediaContentRatingGermany
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5dd25a8bd29211fd593daf3ecea20a7808384bc1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860001"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="48cd3-103">Tipo de recurso mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="48cd3-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="48cd3-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="48cd3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="48cd3-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="48cd3-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="48cd3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="48cd3-106">Properties</span></span>
|<span data-ttu-id="48cd3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="48cd3-107">Property</span></span>|<span data-ttu-id="48cd3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="48cd3-108">Type</span></span>|<span data-ttu-id="48cd3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="48cd3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48cd3-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="48cd3-110">movieRating</span></span>|[<span data-ttu-id="48cd3-111">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="48cd3-111">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="48cd3-112">Filmes classificação selecionado para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="48cd3-112">Movies rating selected for Germany.</span></span> <span data-ttu-id="48cd3-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="48cd3-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="48cd3-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="48cd3-114">tvRating</span></span>|[<span data-ttu-id="48cd3-115">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="48cd3-115">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="48cd3-116">Classificação de TV selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="48cd3-116">TV rating selected for Germany.</span></span> <span data-ttu-id="48cd3-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="48cd3-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48cd3-118">Relações</span><span class="sxs-lookup"><span data-stu-id="48cd3-118">Relationships</span></span>
<span data-ttu-id="48cd3-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="48cd3-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="48cd3-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="48cd3-120">JSON Representation</span></span>
<span data-ttu-id="48cd3-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="48cd3-121">Here is a JSON representation of the resource.</span></span>
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



