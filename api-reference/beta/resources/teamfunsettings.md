---
title: tipo de recurso de teamFunSettings
description: Configurações para configurar o uso de Giphy, memes e adesivos na equipe de.
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: dc8d4cfa05f7bc6cbda9dfbf5d113370a1981ba5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515857"
---
# <a name="teamfunsettings-resource-type"></a><span data-ttu-id="11704-103">tipo de recurso de teamFunSettings</span><span class="sxs-lookup"><span data-stu-id="11704-103">teamFunSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11704-104">Configurações para configurar o uso de Giphy, adesivos e memes em [equipe](team.md).</span><span class="sxs-lookup"><span data-stu-id="11704-104">Settings to configure use of Giphy, memes, and stickers in the [team](team.md).</span></span>

## <a name="properties"></a><span data-ttu-id="11704-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="11704-105">Properties</span></span>
| <span data-ttu-id="11704-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="11704-106">Property</span></span>     | <span data-ttu-id="11704-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="11704-107">Type</span></span>   |<span data-ttu-id="11704-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="11704-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11704-109">allowGiphy</span><span class="sxs-lookup"><span data-stu-id="11704-109">allowGiphy</span></span>|<span data-ttu-id="11704-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="11704-110">Boolean</span></span>|<span data-ttu-id="11704-111">Se definido como true, permite que o uso de Giphy.</span><span class="sxs-lookup"><span data-stu-id="11704-111">If set to true, enables Giphy use.</span></span>|
|<span data-ttu-id="11704-112">giphyContentRating</span><span class="sxs-lookup"><span data-stu-id="11704-112">giphyContentRating</span></span>|<span data-ttu-id="11704-113">Cadeia de caracteres (enum)</span><span class="sxs-lookup"><span data-stu-id="11704-113">String (enum)</span></span>|<span data-ttu-id="11704-114">Classificação de conteúdo Giphy.</span><span class="sxs-lookup"><span data-stu-id="11704-114">Giphy content rating.</span></span> <span data-ttu-id="11704-115">Os valores possíveis são: `moderate` e `strict`.</span><span class="sxs-lookup"><span data-stu-id="11704-115">Possible values are: `moderate`, `strict`.</span></span>|
|<span data-ttu-id="11704-116">allowStickersAndMemes</span><span class="sxs-lookup"><span data-stu-id="11704-116">allowStickersAndMemes</span></span>|<span data-ttu-id="11704-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="11704-117">Boolean</span></span>|<span data-ttu-id="11704-118">Se definido como true, permite que os usuários incluem adesivos e memes.</span><span class="sxs-lookup"><span data-stu-id="11704-118">If set to true, enables users to include stickers and memes.</span></span>|
|<span data-ttu-id="11704-119">allowCustomMemes</span><span class="sxs-lookup"><span data-stu-id="11704-119">allowCustomMemes</span></span>|<span data-ttu-id="11704-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="11704-120">Boolean</span></span>|<span data-ttu-id="11704-121">Se definido como true, permite que os usuários incluem memes personalizado.</span><span class="sxs-lookup"><span data-stu-id="11704-121">If set to true, enables users to include custom memes.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="11704-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="11704-122">JSON representation</span></span>

<span data-ttu-id="11704-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="11704-123">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/teamfunsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
