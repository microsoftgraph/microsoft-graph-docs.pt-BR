---
title: Tipo de recurso mediaContentRatingCanada
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1c0e524e478e89c6d9d6622d727cf9a529614cfe
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43437234"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="9ea54-103">Tipo de recurso mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="9ea54-103">mediaContentRatingCanada resource type</span></span>

<span data-ttu-id="9ea54-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ea54-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ea54-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9ea54-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ea54-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9ea54-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ea54-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="9ea54-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="9ea54-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9ea54-108">Properties</span></span>
|<span data-ttu-id="9ea54-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ea54-109">Property</span></span>|<span data-ttu-id="9ea54-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ea54-110">Type</span></span>|<span data-ttu-id="9ea54-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ea54-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ea54-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="9ea54-112">movieRating</span></span>|[<span data-ttu-id="9ea54-113">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="9ea54-113">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="9ea54-114">Classificação de filmes selecionada para o Canadá.</span><span class="sxs-lookup"><span data-stu-id="9ea54-114">Movies rating selected for Canada.</span></span> <span data-ttu-id="9ea54-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="9ea54-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="9ea54-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="9ea54-116">tvRating</span></span>|[<span data-ttu-id="9ea54-117">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="9ea54-117">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="9ea54-118">Classificação de TV selecionada para o Canadá.</span><span class="sxs-lookup"><span data-stu-id="9ea54-118">TV rating selected for Canada.</span></span> <span data-ttu-id="9ea54-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="9ea54-119">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9ea54-120">Relações</span><span class="sxs-lookup"><span data-stu-id="9ea54-120">Relationships</span></span>
<span data-ttu-id="9ea54-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9ea54-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9ea54-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ea54-122">JSON Representation</span></span>
<span data-ttu-id="9ea54-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9ea54-123">Here is a JSON representation of the resource.</span></span>
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



