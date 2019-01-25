---
title: Tipo de recurso itemBody
description: Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.
localization_priority: Normal
ms.openlocfilehash: f316beda82f292e62d5063f45363e08eeeff7111
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526141"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="179a1-103">Tipo de recurso itemBody</span><span class="sxs-lookup"><span data-stu-id="179a1-103">itemBody resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="179a1-104">Representa as propriedades do corpo de um item, como uma mensagem, um evento ou uma postagem de grupo.</span><span class="sxs-lookup"><span data-stu-id="179a1-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="179a1-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="179a1-105">Properties</span></span>
| <span data-ttu-id="179a1-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="179a1-106">Property</span></span>     | <span data-ttu-id="179a1-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="179a1-107">Type</span></span>   |<span data-ttu-id="179a1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="179a1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="179a1-109">content</span><span class="sxs-lookup"><span data-stu-id="179a1-109">content</span></span>|<span data-ttu-id="179a1-110">String</span><span class="sxs-lookup"><span data-stu-id="179a1-110">String</span></span>|<span data-ttu-id="179a1-111">O conteúdo do item.</span><span class="sxs-lookup"><span data-stu-id="179a1-111">The content of the item.</span></span>|
|<span data-ttu-id="179a1-112">contentType</span><span class="sxs-lookup"><span data-stu-id="179a1-112">contentType</span></span>|<span data-ttu-id="179a1-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="179a1-113">String</span></span>|<span data-ttu-id="179a1-p101">O tipo de conteúdo. Os valores possíveis são: `Text` e `HTML`.</span><span class="sxs-lookup"><span data-stu-id="179a1-p101">The type of the content. Possible values are `Text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="179a1-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="179a1-116">JSON representation</span></span>

<span data-ttu-id="179a1-117">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="179a1-117">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemBody"
}-->

```json
{
  "content": "string",
  "contentType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "itemBody resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/itembody.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
