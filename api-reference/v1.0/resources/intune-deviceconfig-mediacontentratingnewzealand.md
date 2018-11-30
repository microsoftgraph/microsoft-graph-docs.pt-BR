---
title: Tipo de recurso mediaContentRatingNewZealand
description: Ainda não documentado
ms.openlocfilehash: 0d34843ef7cc624b222694cc8fbe0fa7a7c1b74c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005233"
---
# <a name="mediacontentratingnewzealand-resource-type"></a><span data-ttu-id="ac0a2-103">Tipo de recurso mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="ac0a2-103">mediaContentRatingNewZealand resource type</span></span>

> <span data-ttu-id="ac0a2-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ac0a2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ac0a2-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="ac0a2-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="ac0a2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac0a2-106">Properties</span></span>
|<span data-ttu-id="ac0a2-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac0a2-107">Property</span></span>|<span data-ttu-id="ac0a2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac0a2-108">Type</span></span>|<span data-ttu-id="ac0a2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac0a2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac0a2-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="ac0a2-110">movieRating</span></span>|[<span data-ttu-id="ac0a2-111">ratingNewZealandMoviesType</span><span class="sxs-lookup"><span data-stu-id="ac0a2-111">ratingNewZealandMoviesType</span></span>](../resources/intune-deviceconfig-ratingnewzealandmoviestype.md)|<span data-ttu-id="ac0a2-112">Filmes selecionado para a Nova Zelândia de classificação.</span><span class="sxs-lookup"><span data-stu-id="ac0a2-112">Movies rating selected for New Zealand.</span></span> <span data-ttu-id="ac0a2-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span><span class="sxs-lookup"><span data-stu-id="ac0a2-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove13`, `agesAbove15`, `agesAbove16`, `agesAbove18`, `restricted`, `agesAbove16Restricted`.</span></span>|
|<span data-ttu-id="ac0a2-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="ac0a2-114">tvRating</span></span>|[<span data-ttu-id="ac0a2-115">ratingNewZealandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="ac0a2-115">ratingNewZealandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingnewzealandtelevisiontype.md)|<span data-ttu-id="ac0a2-116">Classificação de TV selecionada para a Nova Zelândia.</span><span class="sxs-lookup"><span data-stu-id="ac0a2-116">TV rating selected for New Zealand.</span></span> <span data-ttu-id="ac0a2-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="ac0a2-117">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ac0a2-118">Relações</span><span class="sxs-lookup"><span data-stu-id="ac0a2-118">Relationships</span></span>
<span data-ttu-id="ac0a2-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ac0a2-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ac0a2-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac0a2-120">JSON Representation</span></span>
<span data-ttu-id="ac0a2-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ac0a2-121">Here is a JSON representation of the resource.</span></span>
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



