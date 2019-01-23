---
title: Tipo de recurso mediaContentRatingUnitedStates
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 60f673e31014eb4da027a58ea29099d9d8aa18e3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425831"
---
# <a name="mediacontentratingunitedstates-resource-type"></a><span data-ttu-id="7a581-103">Tipo de recurso mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="7a581-103">mediaContentRatingUnitedStates resource type</span></span>

> <span data-ttu-id="7a581-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="7a581-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7a581-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7a581-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a581-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="7a581-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a581-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7a581-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="7a581-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a581-108">Properties</span></span>
|<span data-ttu-id="7a581-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a581-109">Property</span></span>|<span data-ttu-id="7a581-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a581-110">Type</span></span>|<span data-ttu-id="7a581-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a581-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a581-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="7a581-112">movieRating</span></span>|[<span data-ttu-id="7a581-113">ratingUnitedStatesMoviesType</span><span class="sxs-lookup"><span data-stu-id="7a581-113">ratingUnitedStatesMoviesType</span></span>](../resources/intune-deviceconfig-ratingunitedstatesmoviestype.md)|<span data-ttu-id="7a581-114">Filmes classificação selecionado para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="7a581-114">Movies rating selected for United States.</span></span> <span data-ttu-id="7a581-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="7a581-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `parentalGuidance13`, `restricted`, `adults`.</span></span>|
|<span data-ttu-id="7a581-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="7a581-116">tvRating</span></span>|[<span data-ttu-id="7a581-117">ratingUnitedStatesTelevisionType</span><span class="sxs-lookup"><span data-stu-id="7a581-117">ratingUnitedStatesTelevisionType</span></span>](../resources/intune-deviceconfig-ratingunitedstatestelevisiontype.md)|<span data-ttu-id="7a581-118">Classificação de TV selecionada para os Estados Unidos.</span><span class="sxs-lookup"><span data-stu-id="7a581-118">TV rating selected for United States.</span></span> <span data-ttu-id="7a581-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="7a581-119">Possible values are: `allAllowed`, `allBlocked`, `childrenAll`, `childrenAbove7`, `general`, `parentalGuidance`, `childrenAbove14`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7a581-120">Relações</span><span class="sxs-lookup"><span data-stu-id="7a581-120">Relationships</span></span>
<span data-ttu-id="7a581-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7a581-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7a581-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a581-122">JSON Representation</span></span>
<span data-ttu-id="7a581-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7a581-123">Here is a JSON representation of the resource.</span></span>
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




