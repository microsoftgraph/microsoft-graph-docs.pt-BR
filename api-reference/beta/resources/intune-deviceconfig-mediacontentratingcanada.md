---
title: Tipo de recurso mediaContentRatingCanada
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 503218cf76d235f4122e36d1d358dce9a76e0fda
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572805"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="6178d-103">Tipo de recurso mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="6178d-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="6178d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6178d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6178d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6178d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6178d-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6178d-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6178d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6178d-107">Properties</span></span>
|<span data-ttu-id="6178d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6178d-108">Property</span></span>|<span data-ttu-id="6178d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6178d-109">Type</span></span>|<span data-ttu-id="6178d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6178d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6178d-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="6178d-111">movieRating</span></span>|[<span data-ttu-id="6178d-112">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="6178d-112">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="6178d-113">Classificação de filmes selecionada para o Canadá.</span><span class="sxs-lookup"><span data-stu-id="6178d-113">Movies rating selected for Canada.</span></span> <span data-ttu-id="6178d-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="6178d-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="6178d-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="6178d-115">tvRating</span></span>|[<span data-ttu-id="6178d-116">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="6178d-116">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="6178d-117">Classificação de TV selecionada para o Canadá.</span><span class="sxs-lookup"><span data-stu-id="6178d-117">TV rating selected for Canada.</span></span> <span data-ttu-id="6178d-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="6178d-118">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6178d-119">Relações</span><span class="sxs-lookup"><span data-stu-id="6178d-119">Relationships</span></span>
<span data-ttu-id="6178d-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6178d-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6178d-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6178d-121">JSON Representation</span></span>
<span data-ttu-id="6178d-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6178d-122">Here is a JSON representation of the resource.</span></span>
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





