---
title: Tipo de recurso mediaContentRatingIreland
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9516c98350c239393e735008e91d966f8c6ae7a2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27957995"
---
# <a name="mediacontentratingireland-resource-type"></a><span data-ttu-id="385b1-103">Tipo de recurso mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="385b1-103">mediaContentRatingIreland resource type</span></span>

> <span data-ttu-id="385b1-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="385b1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="385b1-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="385b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="385b1-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="385b1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="385b1-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="385b1-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="385b1-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="385b1-108">Properties</span></span>
|<span data-ttu-id="385b1-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="385b1-109">Property</span></span>|<span data-ttu-id="385b1-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="385b1-110">Type</span></span>|<span data-ttu-id="385b1-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="385b1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="385b1-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="385b1-112">movieRating</span></span>|[<span data-ttu-id="385b1-113">ratingIrelandMoviesType</span><span class="sxs-lookup"><span data-stu-id="385b1-113">ratingIrelandMoviesType</span></span>](../resources/intune-deviceconfig-ratingirelandmoviestype.md)|<span data-ttu-id="385b1-114">Filmes selecionado para Irlanda de classificação.</span><span class="sxs-lookup"><span data-stu-id="385b1-114">Movies rating selected for Ireland.</span></span> <span data-ttu-id="385b1-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="385b1-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove12`, `agesAbove15`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="385b1-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="385b1-116">tvRating</span></span>|[<span data-ttu-id="385b1-117">ratingIrelandTelevisionType</span><span class="sxs-lookup"><span data-stu-id="385b1-117">ratingIrelandTelevisionType</span></span>](../resources/intune-deviceconfig-ratingirelandtelevisiontype.md)|<span data-ttu-id="385b1-118">Classificação de TV selecionada para Irlanda.</span><span class="sxs-lookup"><span data-stu-id="385b1-118">TV rating selected for Ireland.</span></span> <span data-ttu-id="385b1-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span><span class="sxs-lookup"><span data-stu-id="385b1-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `children`, `youngAdults`, `parentalSupervision`, `mature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="385b1-120">Relações</span><span class="sxs-lookup"><span data-stu-id="385b1-120">Relationships</span></span>
<span data-ttu-id="385b1-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="385b1-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="385b1-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="385b1-122">JSON Representation</span></span>
<span data-ttu-id="385b1-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="385b1-123">Here is a JSON representation of the resource.</span></span>
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





