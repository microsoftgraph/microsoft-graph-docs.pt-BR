---
title: Tipo de recurso mediaContentRatingJapan
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2b1ab45a91fb617412742481639a0203624bc11d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945920"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="1d498-103">Tipo de recurso mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="1d498-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="1d498-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1d498-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d498-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1d498-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="1d498-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d498-106">Properties</span></span>
|<span data-ttu-id="1d498-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d498-107">Property</span></span>|<span data-ttu-id="1d498-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d498-108">Type</span></span>|<span data-ttu-id="1d498-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d498-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d498-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="1d498-110">movieRating</span></span>|[<span data-ttu-id="1d498-111">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="1d498-111">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="1d498-112">Filmes classificação selecionado para japonês.</span><span class="sxs-lookup"><span data-stu-id="1d498-112">Movies rating selected for Japan.</span></span> <span data-ttu-id="1d498-113">Os possíveis valores são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="1d498-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="1d498-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="1d498-114">tvRating</span></span>|[<span data-ttu-id="1d498-115">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="1d498-115">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="1d498-116">Classificação de TV selecionada para japonês.</span><span class="sxs-lookup"><span data-stu-id="1d498-116">TV rating selected for Japan.</span></span> <span data-ttu-id="1d498-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="1d498-117">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d498-118">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="1d498-118">Relationships</span></span>
<span data-ttu-id="1d498-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1d498-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1d498-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d498-120">JSON Representation</span></span>
<span data-ttu-id="1d498-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d498-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```



