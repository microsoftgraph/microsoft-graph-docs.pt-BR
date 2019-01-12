---
title: tipo de recurso de teamFunSettings
description: Configurações para configurar o uso de Giphy, memes e adesivos na equipe de.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: c701ffe76c82a6cb4b3586272926290f634a02d9
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987668"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="7445b-103">tipo de recurso de teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="7445b-103">teamFunSettings resource type</span></span>



<span data-ttu-id="7445b-104">Configurações para configurar o uso de Giphy, adesivos e memes em [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="7445b-104">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7445b-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7445b-105">Properties</span></span>
| <span data-ttu-id="7445b-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7445b-106">Property</span></span>     | <span data-ttu-id="7445b-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="7445b-107">Type</span></span>   |<span data-ttu-id="7445b-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7445b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7445b-109">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="7445b-109">allowGiphy</span></span>|<span data-ttu-id="7445b-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="7445b-110">Boolean</span></span>|<span data-ttu-id="7445b-111">Se definido como true, permite que o uso de Giphy.</span><span class="sxs-lookup"><span data-stu-id="7445b-111">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="7445b-112">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="7445b-112">giphyContentRating</span></span>|<span data-ttu-id="7445b-113">Cadeia de caracteres (enum)</span><span class="sxs-lookup"><span data-stu-id="7445b-113">String (enum)</span></span>|<span data-ttu-id="7445b-114">Classificação de conteúdo Giphy.</span><span class="sxs-lookup"><span data-stu-id="7445b-114">Giphy content rating.</span></span> <span data-ttu-id="7445b-115">Os valores possíveis são: `moderate` e `strict`.</span><span class="sxs-lookup"><span data-stu-id="7445b-115">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="7445b-116">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="7445b-116">allowStickersAndMemes</span></span>|<span data-ttu-id="7445b-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="7445b-117">Boolean</span></span>|<span data-ttu-id="7445b-118">Se definido como true, permite que os usuários incluem adesivos e memes.</span><span class="sxs-lookup"><span data-stu-id="7445b-118">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="7445b-119">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="7445b-119">allowCustomMemes</span></span>|<span data-ttu-id="7445b-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="7445b-120">Boolean</span></span>|<span data-ttu-id="7445b-121">Se definido como true, permite que os usuários incluem memes personalizado.</span><span class="sxs-lookup"><span data-stu-id="7445b-121">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7445b-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7445b-122">JSON representation</span></span>

<span data-ttu-id="7445b-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7445b-123">The following is a JSON representation of the resource.</span></span>

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
