---
title: Tipo de recurso mediaContentRatingCanada
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9b4151b810fcfbc56c652492fff9fa1f3f841189
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932179"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="f39bf-103">Tipo de recurso mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="f39bf-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="f39bf-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f39bf-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f39bf-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f39bf-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="f39bf-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f39bf-106">Properties</span></span>
|<span data-ttu-id="f39bf-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f39bf-107">Property</span></span>|<span data-ttu-id="f39bf-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f39bf-108">Type</span></span>|<span data-ttu-id="f39bf-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f39bf-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f39bf-110">movieRating</span><span class="sxs-lookup"><span data-stu-id="f39bf-110">movieRating</span></span>|[<span data-ttu-id="f39bf-111">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="f39bf-111">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="f39bf-112">Filmes classificação selecionado no Canadá.</span><span class="sxs-lookup"><span data-stu-id="f39bf-112">Movies rating selected for Canada.</span></span> <span data-ttu-id="f39bf-113">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="f39bf-113">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="f39bf-114">tvRating</span><span class="sxs-lookup"><span data-stu-id="f39bf-114">tvRating</span></span>|[<span data-ttu-id="f39bf-115">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="f39bf-115">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="f39bf-116">Classificação de TV selecionada para Canadá.</span><span class="sxs-lookup"><span data-stu-id="f39bf-116">TV rating selected for Canada.</span></span> <span data-ttu-id="f39bf-117">Os valores possíveis são: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="f39bf-117">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f39bf-118">Relações</span><span class="sxs-lookup"><span data-stu-id="f39bf-118">Relationships</span></span>
<span data-ttu-id="f39bf-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f39bf-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f39bf-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f39bf-120">JSON Representation</span></span>
<span data-ttu-id="f39bf-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f39bf-121">Here is a JSON representation of the resource.</span></span>
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



