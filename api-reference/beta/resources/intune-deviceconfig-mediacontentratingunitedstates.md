---
title: Tipo de recurso mediaContentRatingUnitedStates
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: ee10df5dd5e3f915e166cb77e747f8b3f7cc2d37
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341318"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="2fee7-103">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="2fee7-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="2fee7-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2fee7-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2fee7-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2fee7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2fee7-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2fee7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2fee7-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="2fee7-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="2fee7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2fee7-108">Properties</span></span>
|<span data-ttu-id="2fee7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2fee7-109">Property</span></span>|<span data-ttu-id="2fee7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2fee7-110">Type</span></span>|<span data-ttu-id="2fee7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2fee7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fee7-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="2fee7-112">movieRating</span></span>|[<span data-ttu-id="2fee7-113">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="2fee7-113">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="2fee7-114">Filmes classificação selecionado para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="2fee7-114">Movies rating selected for United States.</span></span> <span data-ttu-id="2fee7-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="2fee7-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="2fee7-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="2fee7-116">tvRating</span></span>|[<span data-ttu-id="2fee7-117">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="2fee7-117">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="2fee7-118">Classificação de TV selecionada para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="2fee7-118">TV rating selected for United States.</span></span> <span data-ttu-id="2fee7-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="2fee7-119">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fee7-120">Relações</span><span class="sxs-lookup"><span data-stu-id="2fee7-120">Relationships</span></span>
<span data-ttu-id="2fee7-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2fee7-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2fee7-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2fee7-122">JSON Representation</span></span>
<span data-ttu-id="2fee7-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2fee7-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingUnitedStates",
  "movieRating": "String",
  "tvRating": "String"
}
```





