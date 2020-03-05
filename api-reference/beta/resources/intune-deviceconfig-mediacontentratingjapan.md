---
title: Tipo de recurso mediaContentRatingJapan
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bb95139301aecd9bce4f19eac0159a5fe64d92f1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526024"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="cd2b2-103">Tipo de recurso mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="cd2b2-103">mediaContentRatingJapan resource type</span></span>

<span data-ttu-id="cd2b2-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cd2b2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cd2b2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cd2b2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd2b2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cd2b2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd2b2-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cd2b2-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="cd2b2-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cd2b2-108">Properties</span></span>
|<span data-ttu-id="cd2b2-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cd2b2-109">Property</span></span>|<span data-ttu-id="cd2b2-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="cd2b2-110">Type</span></span>|<span data-ttu-id="cd2b2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd2b2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd2b2-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="cd2b2-112">movieRating</span></span>|[<span data-ttu-id="cd2b2-113">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="cd2b2-113">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="cd2b2-114">Classificação de filmes selecionada para o Japão.</span><span class="sxs-lookup"><span data-stu-id="cd2b2-114">Movies rating selected for Japan.</span></span> <span data-ttu-id="cd2b2-115">Os possíveis valores são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="cd2b2-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="cd2b2-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="cd2b2-116">tvRating</span></span>|[<span data-ttu-id="cd2b2-117">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="cd2b2-117">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="cd2b2-118">Classificação de TV selecionada para o Japão.</span><span class="sxs-lookup"><span data-stu-id="cd2b2-118">TV rating selected for Japan.</span></span> <span data-ttu-id="cd2b2-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="cd2b2-119">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd2b2-120">Relações</span><span class="sxs-lookup"><span data-stu-id="cd2b2-120">Relationships</span></span>
<span data-ttu-id="cd2b2-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cd2b2-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd2b2-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cd2b2-122">JSON Representation</span></span>
<span data-ttu-id="cd2b2-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cd2b2-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mediaContentRatingJapan"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mediaContentRatingJapan",
  "movieRating": "String",
  "tvRating": "String"
}
```



