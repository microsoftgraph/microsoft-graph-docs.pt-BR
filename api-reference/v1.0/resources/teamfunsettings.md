---
title: tipo de recurso teamFunSettings
description: Configurações que definem o uso de Giphy, memes e figurinhas na equipe.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 25f49eaff6485fd0d618a91ef942bc2dccf8c8da
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094026"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="ba973-103">tipo de recurso teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="ba973-103">teamFunSettings resource type</span></span>

<span data-ttu-id="ba973-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba973-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="ba973-105">Configurações para configurar o uso de Giphy, memes e selos na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="ba973-105">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ba973-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ba973-106">Properties</span></span>
| <span data-ttu-id="ba973-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ba973-107">Property</span></span>     | <span data-ttu-id="ba973-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="ba973-108">Type</span></span>   |<span data-ttu-id="ba973-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba973-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba973-110">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="ba973-110">allowGiphy</span></span>|<span data-ttu-id="ba973-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="ba973-111">Boolean</span></span>|<span data-ttu-id="ba973-112">Se definido como true, habilita o uso do Giphy.</span><span class="sxs-lookup"><span data-stu-id="ba973-112">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="ba973-113">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="ba973-113">giphyContentRating</span></span>|<span data-ttu-id="ba973-114">Cadeia de caracteres (enum)</span><span class="sxs-lookup"><span data-stu-id="ba973-114">String (enum)</span></span>|<span data-ttu-id="ba973-115">Classificação de conteúdo do Giphy.</span><span class="sxs-lookup"><span data-stu-id="ba973-115">Giphy content rating.</span></span> <span data-ttu-id="ba973-116">Os valores possíveis são: `moderate` e `strict`.</span><span class="sxs-lookup"><span data-stu-id="ba973-116">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="ba973-117">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="ba973-117">allowStickersAndMemes</span></span>|<span data-ttu-id="ba973-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="ba973-118">Boolean</span></span>|<span data-ttu-id="ba973-119">Se definido como true, permite que os usuários incluam adesivos e memes.</span><span class="sxs-lookup"><span data-stu-id="ba973-119">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="ba973-120">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="ba973-120">allowCustomMemes</span></span>|<span data-ttu-id="ba973-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="ba973-121">Boolean</span></span>|<span data-ttu-id="ba973-122">Se definido como true, permite que os usuários incluam memes personalizados.</span><span class="sxs-lookup"><span data-stu-id="ba973-122">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ba973-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ba973-123">JSON representation</span></span>

<span data-ttu-id="ba973-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ba973-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamFunSettings"
}-->

```json
{
  "allowGiphy": true,
  "giphyContentRating": "strict",
  "allowStickersAndMemes": true,
  "allowCustomMemes": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

