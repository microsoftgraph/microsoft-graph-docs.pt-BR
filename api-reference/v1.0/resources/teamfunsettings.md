---
title: tipo de recurso teamFunSettings
description: Configurações que definem o uso de Giphy, memes e figurinhas na equipe.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 696a6a3b02f90abe1456f99d9a40a4d9127b5697
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533544"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="b4870-103">tipo de recurso teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="b4870-103">teamFunSettings resource type</span></span>

<span data-ttu-id="b4870-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4870-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="b4870-105">Configurações para configurar o uso de Giphy, memes e selos na [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="b4870-105">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b4870-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b4870-106">Properties</span></span>
| <span data-ttu-id="b4870-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b4870-107">Property</span></span>     | <span data-ttu-id="b4870-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="b4870-108">Type</span></span>   |<span data-ttu-id="b4870-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="b4870-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4870-110">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="b4870-110">allowGiphy</span></span>|<span data-ttu-id="b4870-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="b4870-111">Boolean</span></span>|<span data-ttu-id="b4870-112">Se definido como true, habilita o uso do Giphy.</span><span class="sxs-lookup"><span data-stu-id="b4870-112">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="b4870-113">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="b4870-113">giphyContentRating</span></span>|<span data-ttu-id="b4870-114">Cadeia de caracteres (enum)</span><span class="sxs-lookup"><span data-stu-id="b4870-114">String (enum)</span></span>|<span data-ttu-id="b4870-115">Classificação de conteúdo do Giphy.</span><span class="sxs-lookup"><span data-stu-id="b4870-115">Giphy content rating.</span></span> <span data-ttu-id="b4870-116">Os valores possíveis são: `moderate` e `strict`.</span><span class="sxs-lookup"><span data-stu-id="b4870-116">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="b4870-117">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="b4870-117">allowStickersAndMemes</span></span>|<span data-ttu-id="b4870-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="b4870-118">Boolean</span></span>|<span data-ttu-id="b4870-119">Se definido como true, permite que os usuários incluam adesivos e memes.</span><span class="sxs-lookup"><span data-stu-id="b4870-119">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="b4870-120">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="b4870-120">allowCustomMemes</span></span>|<span data-ttu-id="b4870-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="b4870-121">Boolean</span></span>|<span data-ttu-id="b4870-122">Se definido como true, permite que os usuários incluam memes personalizados.</span><span class="sxs-lookup"><span data-stu-id="b4870-122">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b4870-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b4870-123">JSON representation</span></span>

<span data-ttu-id="b4870-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b4870-124">The following is a JSON representation of the resource.</span></span>

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
