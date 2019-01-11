---
title: Tipo de recurso mediaContentRatingUnitedStates
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8bce2e359627ede66f32d696c8a84d2ba9faccec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811652"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="838db-103">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="838db-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="838db-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="838db-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="838db-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="838db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="838db-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="838db-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="838db-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="838db-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="838db-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="838db-108">Properties</span></span>
|<span data-ttu-id="838db-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="838db-109">Property</span></span>|<span data-ttu-id="838db-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="838db-110">Type</span></span>|<span data-ttu-id="838db-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="838db-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="838db-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="838db-112">movieRating</span></span>|[<span data-ttu-id="838db-113">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="838db-113">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="838db-114">Filmes classificação selecionado para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="838db-114">Movies rating selected for United States.</span></span> <span data-ttu-id="838db-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="838db-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="838db-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="838db-116">tvRating</span></span>|[<span data-ttu-id="838db-117">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="838db-117">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="838db-118">Classificação de TV selecionada para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="838db-118">TV rating selected for United States.</span></span> <span data-ttu-id="838db-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="838db-119">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="838db-120">Relações</span><span class="sxs-lookup"><span data-stu-id="838db-120">Relationships</span></span>
<span data-ttu-id="838db-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="838db-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="838db-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="838db-122">JSON Representation</span></span>
<span data-ttu-id="838db-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="838db-123">Here is a JSON representation of the resource.</span></span>
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





