---
title: Tipo de recurso mediaContentRatingCanada
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eff3a957e242dfad4840ad5d616cec54f9a3c344
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755039"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="438c1-103">Tipo de recurso mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="438c1-103">mediaContentRatingCanada resource type</span></span>

<span data-ttu-id="438c1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="438c1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="438c1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="438c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="438c1-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="438c1-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="438c1-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="438c1-107">Properties</span></span>
|<span data-ttu-id="438c1-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="438c1-108">Property</span></span>|<span data-ttu-id="438c1-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="438c1-109">Type</span></span>|<span data-ttu-id="438c1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="438c1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="438c1-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="438c1-111">movieRating</span></span>|[<span data-ttu-id="438c1-112">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="438c1-112">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="438c1-113">Classificação de filmes selecionada para o Canadá.</span><span class="sxs-lookup"><span data-stu-id="438c1-113">Movies rating selected for Canada.</span></span> <span data-ttu-id="438c1-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="438c1-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="438c1-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="438c1-115">tvRating</span></span>|[<span data-ttu-id="438c1-116">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="438c1-116">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="438c1-117">Classificação de TV selecionada para o Canadá.</span><span class="sxs-lookup"><span data-stu-id="438c1-117">TV rating selected for Canada.</span></span> <span data-ttu-id="438c1-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="438c1-118">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="438c1-119">Relações</span><span class="sxs-lookup"><span data-stu-id="438c1-119">Relationships</span></span>
<span data-ttu-id="438c1-120">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="438c1-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="438c1-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="438c1-121">JSON Representation</span></span>
<span data-ttu-id="438c1-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="438c1-122">Here is a JSON representation of the resource.</span></span>
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




