---
title: Tipo de recurso mediaContentRatingGermany
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9f60f7fa3abfd5cb23735ba8d87d492e5b752d16
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945129"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="91a86-103">Tipo de recurso mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="91a86-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="91a86-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="91a86-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91a86-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="91a86-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="91a86-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="91a86-106">Properties</span></span>
|<span data-ttu-id="91a86-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91a86-107">Property</span></span>|<span data-ttu-id="91a86-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="91a86-108">Type</span></span>|<span data-ttu-id="91a86-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="91a86-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91a86-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="91a86-110">movieRating</span></span>|[<span data-ttu-id="91a86-111">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="91a86-111">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="91a86-112">Filmes classificação selecionado para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="91a86-112">Movies rating selected for Germany.</span></span> <span data-ttu-id="91a86-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="91a86-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="91a86-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="91a86-114">tvRating</span></span>|[<span data-ttu-id="91a86-115">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="91a86-115">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="91a86-116">Classificação de TV selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="91a86-116">TV rating selected for Germany.</span></span> <span data-ttu-id="91a86-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="91a86-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91a86-118">Relações</span><span class="sxs-lookup"><span data-stu-id="91a86-118">Relationships</span></span>
<span data-ttu-id="91a86-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="91a86-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="91a86-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="91a86-120">JSON Representation</span></span>
<span data-ttu-id="91a86-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="91a86-121">Here is a JSON representation of the resource.</span></span>
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



