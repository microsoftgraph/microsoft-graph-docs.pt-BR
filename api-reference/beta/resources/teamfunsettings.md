---
title: tipo de recurso teamFunSettings
description: Configurações que definem o uso de Giphy, memes e figurinhas na equipe.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 0f96157072ac7b6de403f82822226f316c8dcd46
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341703"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="96b40-103">tipo de recurso teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="96b40-103">teamFunSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96b40-104">Configurações para configurar o uso de Giphy, memes e selos na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="96b40-104">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="96b40-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="96b40-105">Properties</span></span>
| <span data-ttu-id="96b40-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96b40-106">Property</span></span>     | <span data-ttu-id="96b40-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="96b40-107">Type</span></span>   |<span data-ttu-id="96b40-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="96b40-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96b40-109">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="96b40-109">allowGiphy</span></span>|<span data-ttu-id="96b40-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="96b40-110">Boolean</span></span>|<span data-ttu-id="96b40-111">Se definido como true, habilita o uso do Giphy.</span><span class="sxs-lookup"><span data-stu-id="96b40-111">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="96b40-112">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="96b40-112">giphyContentRating</span></span>|<span data-ttu-id="96b40-113">Cadeia de caracteres (enum)</span><span class="sxs-lookup"><span data-stu-id="96b40-113">String (enum)</span></span>|<span data-ttu-id="96b40-114">Classificação de conteúdo do Giphy.</span><span class="sxs-lookup"><span data-stu-id="96b40-114">Giphy content rating.</span></span> <span data-ttu-id="96b40-115">Os valores possíveis são: `moderate` e `strict`.</span><span class="sxs-lookup"><span data-stu-id="96b40-115">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="96b40-116">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="96b40-116">allowStickersAndMemes</span></span>|<span data-ttu-id="96b40-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="96b40-117">Boolean</span></span>|<span data-ttu-id="96b40-118">Se definido como true, permite que os usuários incluam adesivos e memes.</span><span class="sxs-lookup"><span data-stu-id="96b40-118">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="96b40-119">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="96b40-119">allowCustomMemes</span></span>|<span data-ttu-id="96b40-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="96b40-120">Boolean</span></span>|<span data-ttu-id="96b40-121">Se definido como true, permite que os usuários incluam memes personalizados.</span><span class="sxs-lookup"><span data-stu-id="96b40-121">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="96b40-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="96b40-122">JSON representation</span></span>

<span data-ttu-id="96b40-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="96b40-123">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "team's funSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
