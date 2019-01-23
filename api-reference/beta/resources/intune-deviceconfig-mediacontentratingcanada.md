---
title: Tipo de recurso mediaContentRatingCanada
description: Ainda não documentado
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 292dc926a626a2aca96312133eb6c9a850db39af
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398048"
---
# <a name="mediacontentratingcanada-resource-type"></a><span data-ttu-id="79665-103">Tipo de recurso mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="79665-103">mediaContentRatingCanada resource type</span></span>

> <span data-ttu-id="79665-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="79665-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="79665-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="79665-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="79665-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="79665-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79665-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="79665-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="79665-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79665-108">Properties</span></span>
|<span data-ttu-id="79665-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79665-109">Property</span></span>|<span data-ttu-id="79665-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="79665-110">Type</span></span>|<span data-ttu-id="79665-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="79665-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79665-112">movieRating</span><span class="sxs-lookup"><span data-stu-id="79665-112">movieRating</span></span>|[<span data-ttu-id="79665-113">ratingCanadaMoviesType</span><span class="sxs-lookup"><span data-stu-id="79665-113">ratingCanadaMoviesType</span></span>](../resources/intune-deviceconfig-ratingcanadamoviestype.md)|<span data-ttu-id="79665-114">Filmes classificação selecionado no Canadá.</span><span class="sxs-lookup"><span data-stu-id="79665-114">Movies rating selected for Canada.</span></span> <span data-ttu-id="79665-115">Os valores possíveis são: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span><span class="sxs-lookup"><span data-stu-id="79665-115">Possible values are: `allAllowed`, `allBlocked`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`, `restricted`.</span></span>|
|<span data-ttu-id="79665-116">tvRating</span><span class="sxs-lookup"><span data-stu-id="79665-116">tvRating</span></span>|[<span data-ttu-id="79665-117">ratingCanadaTelevisionType</span><span class="sxs-lookup"><span data-stu-id="79665-117">ratingCanadaTelevisionType</span></span>](../resources/intune-deviceconfig-ratingcanadatelevisiontype.md)|<span data-ttu-id="79665-118">Classificação de TV selecionada para Canadá.</span><span class="sxs-lookup"><span data-stu-id="79665-118">TV rating selected for Canada.</span></span> <span data-ttu-id="79665-119">Os valores possíveis são: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span><span class="sxs-lookup"><span data-stu-id="79665-119">Possible values are: `allAllowed`, `allBlocked`, `children`, `childrenAbove8`, `general`, `parentalGuidance`, `agesAbove14`, `agesAbove18`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79665-120">Relações</span><span class="sxs-lookup"><span data-stu-id="79665-120">Relationships</span></span>
<span data-ttu-id="79665-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="79665-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="79665-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79665-122">JSON Representation</span></span>
<span data-ttu-id="79665-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="79665-123">Here is a JSON representation of the resource.</span></span>
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




