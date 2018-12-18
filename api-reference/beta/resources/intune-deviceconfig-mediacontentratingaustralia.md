---
title: Tipo de recurso mediaContentRatingAustralia
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: 29501d5e52b922baabd777a8838896230a502631
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317161"
---
# <a name="mediacontentratingaustralia-resource-type"></a><span data-ttu-id="cbfb4-103">Tipo de recurso mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="cbfb4-103">mediaContentRatingAustralia resource type</span></span>

> <span data-ttu-id="cbfb4-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cbfb4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cbfb4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cbfb4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cbfb4-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cbfb4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cbfb4-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cbfb4-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="cbfb4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cbfb4-108">Properties</span></span>
|<span data-ttu-id="cbfb4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cbfb4-109">Property</span></span>|<span data-ttu-id="cbfb4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbfb4-110">Type</span></span>|<span data-ttu-id="cbfb4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbfb4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cbfb4-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="cbfb4-112">movieRating</span></span>|[<span data-ttu-id="cbfb4-113">ratingAustraliaMoviesType</span><span class="sxs-lookup"><span data-stu-id="cbfb4-113">ratingAustraliaMoviesType</span></span>](../resources/intune-deviceconfig-ratingaustraliamoviestype.md)|<span data-ttu-id="cbfb4-114">Filmes selecionado para Austrália de classificação.</span><span class="sxs-lookup"><span data-stu-id="cbfb4-114">Movies rating selected for Australia.</span></span> <span data-ttu-id="cbfb4-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="cbfb4-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="cbfb4-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="cbfb4-116">tvRating</span></span>|[<span data-ttu-id="cbfb4-117">ratingAustraliaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="cbfb4-117">ratingAustraliaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingaustraliatelevisiontype.md)|<span data-ttu-id="cbfb4-118">Classificação de TV selecionada para Austrália.</span><span class="sxs-lookup"><span data-stu-id="cbfb4-118">TV rating selected for Australia.</span></span> <span data-ttu-id="cbfb4-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span><span class="sxs-lookup"><span data-stu-id="cbfb4-119">Possible values are: `allAllowed`, `allBlocked`, `preschoolers`, `children`, `general`, `parentalGuidance`, `mature`, `agesAbove15`, `agesAbove15AdultViolence`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cbfb4-120">Relações</span><span class="sxs-lookup"><span data-stu-id="cbfb4-120">Relationships</span></span>
<span data-ttu-id="cbfb4-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cbfb4-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cbfb4-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cbfb4-122">JSON Representation</span></span>
<span data-ttu-id="cbfb4-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cbfb4-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingAustralia"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingAustralia",
  "movieRating": "String",
  "tvRating": "String"
}
```





