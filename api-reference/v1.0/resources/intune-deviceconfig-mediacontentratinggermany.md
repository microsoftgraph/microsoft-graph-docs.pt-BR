---
title: Tipo de recurso mediaContentRatingGermany
description: Ainda não documentado
ms.openlocfilehash: 40ad8d4794b44a41614d9ed02341a00bdb4df86d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005232"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="6c0d6-103">Tipo de recurso mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="6c0d6-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="6c0d6-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6c0d6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c0d6-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6c0d6-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="6c0d6-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6c0d6-106">Properties</span></span>
|<span data-ttu-id="6c0d6-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c0d6-107">Property</span></span>|<span data-ttu-id="6c0d6-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c0d6-108">Type</span></span>|<span data-ttu-id="6c0d6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c0d6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c0d6-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="6c0d6-110">movieRating</span></span>|[<span data-ttu-id="6c0d6-111">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="6c0d6-111">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="6c0d6-112">Filmes classificação selecionado para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="6c0d6-112">Movies rating selected for Germany.</span></span> <span data-ttu-id="6c0d6-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="6c0d6-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="6c0d6-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="6c0d6-114">tvRating</span></span>|[<span data-ttu-id="6c0d6-115">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="6c0d6-115">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="6c0d6-116">Classificação de TV selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="6c0d6-116">TV rating selected for Germany.</span></span> <span data-ttu-id="6c0d6-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="6c0d6-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c0d6-118">Relações</span><span class="sxs-lookup"><span data-stu-id="6c0d6-118">Relationships</span></span>
<span data-ttu-id="6c0d6-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6c0d6-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6c0d6-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6c0d6-120">JSON Representation</span></span>
<span data-ttu-id="6c0d6-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6c0d6-121">Here is a JSON representation of the resource.</span></span>
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



