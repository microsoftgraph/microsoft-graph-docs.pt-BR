---
title: Tipo de recurso mediaContentRatingCanada
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: 310d68ea3ee0fa563b9fe413e26bace51251025a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312492"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="cd7c2-103">Tipo de recurso mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="cd7c2-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="cd7c2-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cd7c2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd7c2-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cd7c2-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="cd7c2-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cd7c2-106">Properties</span></span>
|<span data-ttu-id="cd7c2-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd7c2-107">Property</span></span>|<span data-ttu-id="cd7c2-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd7c2-108">Type</span></span>|<span data-ttu-id="cd7c2-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd7c2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd7c2-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="cd7c2-110">movieRating</span></span>|[<span data-ttu-id="cd7c2-111">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="cd7c2-111">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="cd7c2-112">Filmes classificação selecionado no Canadá.</span><span class="sxs-lookup"><span data-stu-id="cd7c2-112">Movies rating selected for Canada.</span></span> <span data-ttu-id="cd7c2-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="cd7c2-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="cd7c2-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="cd7c2-114">tvRating</span></span>|[<span data-ttu-id="cd7c2-115">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="cd7c2-115">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="cd7c2-116">Classificação de TV selecionada para Canadá.</span><span class="sxs-lookup"><span data-stu-id="cd7c2-116">TV rating selected for Canada.</span></span> <span data-ttu-id="cd7c2-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="cd7c2-117">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd7c2-118">Relações</span><span class="sxs-lookup"><span data-stu-id="cd7c2-118">Relationships</span></span>
<span data-ttu-id="cd7c2-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cd7c2-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cd7c2-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cd7c2-120">JSON Representation</span></span>
<span data-ttu-id="cd7c2-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cd7c2-121">Here is a JSON representation of the resource.</span></span>
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



