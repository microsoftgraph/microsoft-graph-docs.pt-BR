---
title: Tipo de recurso mediaContentRatingIreland
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b3efd96cc8ad015989365dff10b1659ef50c4fb7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29422597"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="32469-103">Tipo de recurso mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="32469-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="32469-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="32469-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="32469-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="32469-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="32469-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="32469-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32469-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="32469-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="32469-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="32469-108">Properties</span></span>
|<span data-ttu-id="32469-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32469-109">Property</span></span>|<span data-ttu-id="32469-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="32469-110">Type</span></span>|<span data-ttu-id="32469-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="32469-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32469-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="32469-112">movieRating</span></span>|[<span data-ttu-id="32469-113">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="32469-113">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="32469-114">Filmes selecionado para Irlanda de classificação.</span><span class="sxs-lookup"><span data-stu-id="32469-114">Movies rating selected for Ireland.</span></span> <span data-ttu-id="32469-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="32469-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="32469-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="32469-116">tvRating</span></span>|[<span data-ttu-id="32469-117">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="32469-117">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="32469-118">Classificação de TV selecionada para Irlanda.</span><span class="sxs-lookup"><span data-stu-id="32469-118">TV rating selected for Ireland.</span></span> <span data-ttu-id="32469-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="32469-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32469-120">Relações</span><span class="sxs-lookup"><span data-stu-id="32469-120">Relationships</span></span>
<span data-ttu-id="32469-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="32469-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32469-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="32469-122">JSON Representation</span></span>
<span data-ttu-id="32469-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="32469-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingIreland"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingIreland",
  "movieRating": "String",
  "tvRating": "String"
}
```




