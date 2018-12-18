---
title: Tipo de recurso mediaContentRatingGermany
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: 8add327725e5d3886d381b63c7debc16c256d810
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327696"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="661e4-103">Tipo de recurso mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="661e4-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="661e4-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="661e4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="661e4-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="661e4-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="661e4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="661e4-106">Properties</span></span>
|<span data-ttu-id="661e4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="661e4-107">Property</span></span>|<span data-ttu-id="661e4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="661e4-108">Type</span></span>|<span data-ttu-id="661e4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="661e4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="661e4-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="661e4-110">movieRating</span></span>|[<span data-ttu-id="661e4-111">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="661e4-111">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="661e4-112">Filmes classificação selecionado para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="661e4-112">Movies rating selected for Germany.</span></span> <span data-ttu-id="661e4-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="661e4-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="661e4-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="661e4-114">tvRating</span></span>|[<span data-ttu-id="661e4-115">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="661e4-115">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="661e4-116">Classificação de TV selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="661e4-116">TV rating selected for Germany.</span></span> <span data-ttu-id="661e4-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="661e4-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="661e4-118">Relações</span><span class="sxs-lookup"><span data-stu-id="661e4-118">Relationships</span></span>
<span data-ttu-id="661e4-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="661e4-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="661e4-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="661e4-120">JSON Representation</span></span>
<span data-ttu-id="661e4-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="661e4-121">Here is a JSON representation of the resource.</span></span>
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



