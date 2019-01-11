---
title: Tipo de recurso mediaContentRatingCanada
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 430baf0e6adaf53d922dc6cf94c8640107869ec4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879930"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="bc114-103">Tipo de recurso mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="bc114-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="bc114-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bc114-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc114-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bc114-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc114-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="bc114-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc114-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bc114-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="bc114-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bc114-108">Properties</span></span>
|<span data-ttu-id="bc114-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc114-109">Property</span></span>|<span data-ttu-id="bc114-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc114-110">Type</span></span>|<span data-ttu-id="bc114-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc114-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc114-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="bc114-112">movieRating</span></span>|[<span data-ttu-id="bc114-113">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="bc114-113">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="bc114-114">Filmes classificação selecionado no Canadá.</span><span class="sxs-lookup"><span data-stu-id="bc114-114">Movies rating selected for Canada.</span></span> <span data-ttu-id="bc114-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="bc114-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="bc114-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="bc114-116">tvRating</span></span>|[<span data-ttu-id="bc114-117">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="bc114-117">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="bc114-118">Classificação de TV selecionada para Canadá.</span><span class="sxs-lookup"><span data-stu-id="bc114-118">TV rating selected for Canada.</span></span> <span data-ttu-id="bc114-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="bc114-119">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc114-120">Relações</span><span class="sxs-lookup"><span data-stu-id="bc114-120">Relationships</span></span>
<span data-ttu-id="bc114-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bc114-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="bc114-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bc114-122">JSON Representation</span></span>
<span data-ttu-id="bc114-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bc114-123">Here is a JSON representation of the resource.</span></span>
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





