---
title: Tipo de recurso mediaContentRatingJapan
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1c129fb2853025758fc71aff381efe500d38ec8f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394835"
---
# <a name="mediacontentratingjapan-resource-type"></a><span data-ttu-id="69554-103">Tipo de recurso mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="69554-103">mediaContentRatingJapan resource type</span></span>

> <span data-ttu-id="69554-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="69554-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="69554-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="69554-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="69554-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="69554-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69554-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="69554-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="69554-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69554-108">Properties</span></span>
|<span data-ttu-id="69554-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="69554-109">Property</span></span>|<span data-ttu-id="69554-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="69554-110">Type</span></span>|<span data-ttu-id="69554-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="69554-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69554-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="69554-112">movieRating</span></span>|[<span data-ttu-id="69554-113">ratingJapanMoviesType</span><span class="sxs-lookup"><span data-stu-id="69554-113">ratingJapanMoviesType</span></span>](../resources/intune-deviceconfig-ratingjapanmoviestype.md)|<span data-ttu-id="69554-114">Filmes classificação selecionado para japonês.</span><span class="sxs-lookup"><span data-stu-id="69554-114">Movies rating selected for Japan.</span></span> <span data-ttu-id="69554-115">Os possíveis valores são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="69554-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove15`, `agesAbove18`.</span></span>|
|<span data-ttu-id="69554-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="69554-116">tvRating</span></span>|[<span data-ttu-id="69554-117">ratingJapanTelevisionType</span><span class="sxs-lookup"><span data-stu-id="69554-117">ratingJapanTelevisionType</span></span>](../resources/intune-deviceconfig-ratingjapantelevisiontype.md)|<span data-ttu-id="69554-118">Classificação de TV selecionada para japonês.</span><span class="sxs-lookup"><span data-stu-id="69554-118">TV rating selected for Japan.</span></span> <span data-ttu-id="69554-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `explicitAllowed`.</span><span class="sxs-lookup"><span data-stu-id="69554-119">Possible values are: `allAllowed`, `allBlocked`, `explicitAllowed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69554-120">Relacionamentos</span><span class="sxs-lookup"><span data-stu-id="69554-120">Relationships</span></span>
<span data-ttu-id="69554-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="69554-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="69554-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69554-122">JSON Representation</span></span>
<span data-ttu-id="69554-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="69554-123">Here is a JSON representation of the resource.</span></span>
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




