---
title: Tipo de recurso mediaContentRatingJapan
description: Ainda não documentado
ms.openlocfilehash: 2fdf6ea6115f066df697a778e44e0476feac7d96
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034843"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="69a4c-103">Tipo de recurso mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="69a4c-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="69a4c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="69a4c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="69a4c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="69a4c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="69a4c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="69a4c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69a4c-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="69a4c-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="69a4c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69a4c-108">Properties</span></span>
|<span data-ttu-id="69a4c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69a4c-109">Property</span></span>|<span data-ttu-id="69a4c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="69a4c-110">Type</span></span>|<span data-ttu-id="69a4c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="69a4c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69a4c-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="69a4c-112">movieRating</span></span>|[<span data-ttu-id="69a4c-113">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="69a4c-113">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="69a4c-114">Filmes classificação selecionado para japonês.</span><span class="sxs-lookup"><span data-stu-id="69a4c-114">Movies rating selected for Japan.</span></span> <span data-ttu-id="69a4c-115">Os possíveis valores são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="69a4c-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="69a4c-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="69a4c-116">tvRating</span></span>|[<span data-ttu-id="69a4c-117">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="69a4c-117">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="69a4c-118">Classificação de TV selecionada para japonês.</span><span class="sxs-lookup"><span data-stu-id="69a4c-118">TV rating selected for Japan.</span></span> <span data-ttu-id="69a4c-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="69a4c-119">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69a4c-120">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="69a4c-120">Relationships</span></span>
<span data-ttu-id="69a4c-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="69a4c-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="69a4c-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69a4c-122">JSON Representation</span></span>
<span data-ttu-id="69a4c-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="69a4c-123">Here is a JSON representation of the resource.</span></span>
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





