---
title: Tipo de recurso mediaContentRatingNewZealand
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5d4a22f9510a615dab746912aed1de5123184ca3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850544"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="4e86f-103">Tipo de recurso mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="4e86f-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="4e86f-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4e86f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e86f-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4e86f-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="4e86f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4e86f-106">Properties</span></span>
|<span data-ttu-id="4e86f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4e86f-107">Property</span></span>|<span data-ttu-id="4e86f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="4e86f-108">Type</span></span>|<span data-ttu-id="4e86f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4e86f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e86f-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="4e86f-110">movieRating</span></span>|[<span data-ttu-id="4e86f-111">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="4e86f-111">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="4e86f-112">Filmes selecionado para a Nova Zelândia de classificação.</span><span class="sxs-lookup"><span data-stu-id="4e86f-112">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="4e86f-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="4e86f-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="4e86f-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="4e86f-114">tvRating</span></span>|[<span data-ttu-id="4e86f-115">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="4e86f-115">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="4e86f-116">Classificação de TV selecionada para a Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="4e86f-116">TV rating selected for New Zealand.</span></span> <span data-ttu-id="4e86f-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="4e86f-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e86f-118">Relações</span><span class="sxs-lookup"><span data-stu-id="4e86f-118">Relationships</span></span>
<span data-ttu-id="4e86f-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4e86f-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4e86f-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4e86f-120">JSON Representation</span></span>
<span data-ttu-id="4e86f-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4e86f-121">Here is a JSON representation of the resource.</span></span>
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



