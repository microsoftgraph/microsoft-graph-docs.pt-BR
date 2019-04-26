---
title: Tipo de recurso mediaContentRatingGermany
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 111abc1804874dd7345d654eafdb1452c05ebd42
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554482"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="f7346-103">Tipo de recurso mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="f7346-103">mediaContentRatingGermany resource type</span></span>

> <span data-ttu-id="f7346-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f7346-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7346-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f7346-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7346-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="f7346-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="f7346-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f7346-107">Properties</span></span>
|<span data-ttu-id="f7346-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7346-108">Property</span></span>|<span data-ttu-id="f7346-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7346-109">Type</span></span>|<span data-ttu-id="f7346-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7346-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7346-111">movieRating</span><span class="sxs-lookup"><span data-stu-id="f7346-111">movieRating</span></span>|[<span data-ttu-id="f7346-112">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="f7346-112">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="f7346-113">Classificação de filmes selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="f7346-113">Movies rating selected for Germany.</span></span> <span data-ttu-id="f7346-114">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="f7346-114">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="f7346-115">tvRating</span><span class="sxs-lookup"><span data-stu-id="f7346-115">tvRating</span></span>|[<span data-ttu-id="f7346-116">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="f7346-116">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="f7346-117">Classificação de TV selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="f7346-117">TV rating selected for Germany.</span></span> <span data-ttu-id="f7346-118">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="f7346-118">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7346-119">Relações</span><span class="sxs-lookup"><span data-stu-id="f7346-119">Relationships</span></span>
<span data-ttu-id="f7346-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f7346-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7346-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f7346-121">JSON Representation</span></span>
<span data-ttu-id="f7346-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f7346-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingGermany"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingGermany",
  "movieRating": "String",
  "tvRating": "String"
}
```





