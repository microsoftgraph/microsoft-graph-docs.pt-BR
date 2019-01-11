---
title: Tipo de recurso mediaContentRatingCanada
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c40691556e9a8f674256c040a98f22e6ef9d717f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857306"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="0a413-103">Tipo de recurso mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="0a413-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="0a413-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0a413-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a413-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="0a413-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="0a413-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0a413-106">Properties</span></span>
|<span data-ttu-id="0a413-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a413-107">Property</span></span>|<span data-ttu-id="0a413-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a413-108">Type</span></span>|<span data-ttu-id="0a413-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a413-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a413-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="0a413-110">movieRating</span></span>|[<span data-ttu-id="0a413-111">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="0a413-111">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="0a413-112">Filmes classificação selecionado no Canadá.</span><span class="sxs-lookup"><span data-stu-id="0a413-112">Movies rating selected for Canada.</span></span> <span data-ttu-id="0a413-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="0a413-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="0a413-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="0a413-114">tvRating</span></span>|[<span data-ttu-id="0a413-115">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="0a413-115">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="0a413-116">Classificação de TV selecionada para Canadá.</span><span class="sxs-lookup"><span data-stu-id="0a413-116">TV rating selected for Canada.</span></span> <span data-ttu-id="0a413-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="0a413-117">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a413-118">Relações</span><span class="sxs-lookup"><span data-stu-id="0a413-118">Relationships</span></span>
<span data-ttu-id="0a413-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0a413-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0a413-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0a413-120">JSON Representation</span></span>
<span data-ttu-id="0a413-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0a413-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingCanada"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingCanada",
  "movieRating": "String",
  "tvRating": "String"
}
```



