---
title: Tipo de recurso mediaContentRatingFrance
description: Ainda não documentado
ms.openlocfilehash: bd2f4933ea05c7db193d700799cdcbdc79490356
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004054"
---
# <a name="mediacontentratingfrance-resource-type"></a><span data-ttu-id="1054a-103">Tipo de recurso mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="1054a-103">mediaContentRatingFrance resource type</span></span>

> <span data-ttu-id="1054a-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1054a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1054a-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1054a-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="1054a-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1054a-106">Properties</span></span>
|<span data-ttu-id="1054a-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1054a-107">Property</span></span>|<span data-ttu-id="1054a-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="1054a-108">Type</span></span>|<span data-ttu-id="1054a-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="1054a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1054a-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="1054a-110">movieRating</span></span>|[<span data-ttu-id="1054a-111">ratingFranceMoviesType</span><span class="sxs-lookup"><span data-stu-id="1054a-111">ratingFranceMoviesType</span></span>](../resources/intune-deviceconfig-ratingfrancemoviestype.md)|<span data-ttu-id="1054a-112">Filmes selecionado de classificação da França.</span><span class="sxs-lookup"><span data-stu-id="1054a-112">Movies rating selected for France.</span></span> <span data-ttu-id="1054a-113">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="1054a-113">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|
|<span data-ttu-id="1054a-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="1054a-114">tvRating</span></span>|[<span data-ttu-id="1054a-115">ratingFranceTelevisionType</span><span class="sxs-lookup"><span data-stu-id="1054a-115">ratingFranceTelevisionType</span></span>](../resources/intune-deviceconfig-ratingfrancetelevisiontype.md)|<span data-ttu-id="1054a-116">Classificação de TV selecionada para França.</span><span class="sxs-lookup"><span data-stu-id="1054a-116">TV rating selected for France.</span></span> <span data-ttu-id="1054a-117">Os possíveis valores são: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="1054a-117">Possible values are: `allAllowed`, `allBlocked`, `agesAbove10`, `agesAbove12`, `agesAbove16`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1054a-118">Relações</span><span class="sxs-lookup"><span data-stu-id="1054a-118">Relationships</span></span>
<span data-ttu-id="1054a-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1054a-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1054a-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1054a-120">JSON Representation</span></span>
<span data-ttu-id="1054a-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1054a-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingFrance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingFrance",
  "movieRating": "String",
  "tvRating": "String"
}
```



