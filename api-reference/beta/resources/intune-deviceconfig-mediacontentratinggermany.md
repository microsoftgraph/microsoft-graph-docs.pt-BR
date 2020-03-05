---
title: Tipo de recurso mediaContentRatingGermany
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d9c55acb14d9e1d184da95a343edac6b3a6dcf4b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526031"
---
# <a name="mediacontentratinggermany-resource-type"></a><span data-ttu-id="c1c26-103">Tipo de recurso mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="c1c26-103">mediaContentRatingGermany resource type</span></span>

<span data-ttu-id="c1c26-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c1c26-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1c26-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c1c26-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1c26-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c1c26-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1c26-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="c1c26-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c1c26-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c1c26-108">Properties</span></span>
|<span data-ttu-id="c1c26-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1c26-109">Property</span></span>|<span data-ttu-id="c1c26-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1c26-110">Type</span></span>|<span data-ttu-id="c1c26-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1c26-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1c26-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="c1c26-112">movieRating</span></span>|[<span data-ttu-id="c1c26-113">ratingGermanyMoviesType</span><span class="sxs-lookup"><span data-stu-id="c1c26-113">ratingGermanyMoviesType</span></span>](../resources/intune-deviceconfig-ratinggermanymoviestype.md)|<span data-ttu-id="c1c26-114">Classificação de filmes selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="c1c26-114">Movies rating selected for Germany.</span></span> <span data-ttu-id="c1c26-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="c1c26-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|
|<span data-ttu-id="c1c26-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="c1c26-116">tvRating</span></span>|[<span data-ttu-id="c1c26-117">ratingGermanyTelevisionType</span><span class="sxs-lookup"><span data-stu-id="c1c26-117">ratingGermanyTelevisionType</span></span>](../resources/intune-deviceconfig-ratinggermanytelevisiontype.md)|<span data-ttu-id="c1c26-118">Classificação de TV selecionada para a Alemanha.</span><span class="sxs-lookup"><span data-stu-id="c1c26-118">TV rating selected for Germany.</span></span> <span data-ttu-id="c1c26-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span><span class="sxs-lookup"><span data-stu-id="c1c26-119">Possible values are: `allAllowed`, `allBlocked`, `general`, `agesAbove6`, `agesAbove12`, `agesAbove16`, `adults`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1c26-120">Relações</span><span class="sxs-lookup"><span data-stu-id="c1c26-120">Relationships</span></span>
<span data-ttu-id="c1c26-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c1c26-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1c26-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c1c26-122">JSON Representation</span></span>
<span data-ttu-id="c1c26-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c1c26-123">Here is a JSON representation of the resource.</span></span>
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



